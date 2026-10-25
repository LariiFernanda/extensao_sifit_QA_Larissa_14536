#Cenário 09: Gerenciamento de Contas a Pagar

---

## Caso de Teste CT01: Cadastrar conta a pagar com dados válidos

| ID | Descrição |
|---|---|
| **C09-CT01** | Verificar se o sistema SIFIT permite cadastrar uma conta a pagar utilizando informações válidas. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT e possuir permissão para cadastrar contas a pagar. Deve existir um fornecedor cadastrado. |

| Passos |
|---|
| DADO que estamos na página de Contas a Pagar |
| E clicamos no botão de cadastrar uma nova conta |
| E informamos o título da despesa |
| E selecionamos um fornecedor cadastrado |
| E preenchemos o tipo de despesa, documento, categoria e local de pagamento conforme os campos exigidos |
| E informamos um valor válido e uma data de vencimento |
| QUANDO clicarmos no botão "Salvar" |
| ENTÃO a conta deverá ser cadastrada e exibida na listagem |

| Critérios de aceitação |
|---|
| O sistema deve cadastrar a conta corretamente, gerar um código de identificação e manter todas as informações vinculadas ao registro. |

| Resultado obtido |
|---|
|Ao preencher todos os capos solicitados, o sistema deu erro na hora de salvar. |

| Status |
|---|
|❌ Reprovado. |

| Evidência(s) |
|---|
|https://jam.dev/c/329cb8b0-c0ea-47e7-8f8c-68188faa48f8|
