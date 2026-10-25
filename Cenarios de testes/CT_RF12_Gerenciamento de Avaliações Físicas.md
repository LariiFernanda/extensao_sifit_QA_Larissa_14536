## Cenário 12: Gerenciamento de Avaliações Físicas

## Caso de Teste CT01: Cadastrar avaliação física com dados válidos

| ID | Descrição |
|---|---|
| **C12-CT01** | Verificar se o sistema SIFIT permite cadastrar uma nova avaliação física utilizando informações válidas. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT e possuir permissão para cadastrar avaliações. Devem existir um aluno e um personal cadastrados e aptos para seleção. |

| Passos |
|---|
| DADO que estamos na página de Avaliações |
| E clicamos no botão "Cadastrar Avaliação" |
| E selecionamos um aluno cadastrado |
| E selecionamos um personal responsável |
| E informamos uma data válida |
| E definimos um horário para a avaliação |
| QUANDO clicarmos no botão "Salvar" |
| ENTÃO o sistema deverá cadastrar a avaliação e exibi-la na listagem |

| Critérios de aceitação |
|---|
| O sistema deve cadastrar a avaliação corretamente, vinculando o aluno ao personal responsável, à data e ao horário selecionados. |

| Resultado obtido |
|---|
| Resultado positivo, como o esperado. |

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
| https://jam.dev/c/32a6b3d9-3947-49a9-b32a-cd42c697b8a6 |
