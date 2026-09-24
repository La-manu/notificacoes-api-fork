# Registro de Testes Unitários
Aluno: Layra Emanuelle Gomes Scarmanha
Grupo: 01
Data: 24/09/2026
## Testes escritos
| # | Arquivo | O que o teste verifica | Tipo |
| --- | ------- | ---------------------- | ----------------------- |
| 1 | validators.test.js| Verifica se um e-mail válido não retorna erro| ✅sucesso |
| 2 | validators.test.js|Verifica se um e-mail sem @ retorna mensagem de erro | ❌falha|
| 3 | validators.test.js| Verifica se um nome com 3 letras não retorna erro| ⚠️borda |
| 4 | validators.test.js| Verifica se um nome com menos de 3 letras retorna mensagem de erro| ⚠️borda|
| 5 | parseId.test.js | Verifica se um ID que não é número lança um ValidationError | ❌Falha|
| 6 | ambiente.test.js | Ambiente de testes está configurado corretamente | ✅Sucesso |
## Resultado
Passaram: Test Suites: 3 passed, 3 total, Tests:       6 passed, 6 total
Falharam: nenhum
## Defeito encontrado
Teste:
Esperado:
Obtido:
## Cobertura
% Lines da linha "helpers": 55,55%

Em uma frase, o que esse número significa:

O **% Lines** indica a porcentagem de linhas do código da pasta `helpers` que foram executadas pelos testes.
