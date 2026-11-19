# Registro de Testes de Endpoint
Aluno: Layra Emanuelle Gomes Scarmanha
Grupo: 01
## Testes escritos
| # | Verbo e rota | Com token? | Status esperado | Verde ou vermelho? |
| --- | ------------ | ---------- | --------------- | ------------------ |
| 1 |	GET /eventos | Não | 200 | 	Verde |
| 2 | 	POST /eventos | Não | 401 | 	Verde |
| 3 | POST /eventos | Sim | 201 | 	Verde |
## Resultado
Linha "Tests:" da saída do npm run test:endpoint:

NB23-2DEV  tsof-aula06  ➜ (main)   24.19.0  ♥ 14:01  npm run test:endpoint

> notificacoes-api@1.0.0 test:endpoint
> jest tests/endpoint --runInBand

 PASS  tests/endpoint/evento.endpoint.test.js

Test Suites: 1 passed, 1 total
Tests:       5 passed, 5 total
Snapshots:   0 total
Time:        1.586 s, estimated 2 s
## Defeito encontrado
Teste: GET /eventos/:id com letras no ID.
Esperado: 400 — Bad Request.
Obtido: 200 — OK, quando as letras são colocadas depois do número do ID, como em /eventos/1abc.
Em qual aula esse mesmo defeito já tinha aparecido, e como: Na aula sobre validação de dados/rotas, o problema apareceu porque o parseInt() converte apenas o começo numérico do texto. Assim, parseInt("1abc") retorna 1, em vez de rejeitar o ID inválido.