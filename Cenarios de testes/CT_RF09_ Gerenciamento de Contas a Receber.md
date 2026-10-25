# Cenário 09: Gerenciamento de Contas a Receber
---

## Caso de Teste CT09: Cadastrar conta a receber com dados válidos

| ID | Descrição |
|---|---|
| **C09-CT01** | Verificar se o sistema SIFIT permite cadastrar uma nova conta a receber utilizando informações válidas. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT, possuir permissão para cadastrar contas a receber e existir um cliente cadastrado. |

| Passos |
|---|
| DADO que estamos na página de Contas a Receber |
| E clicamos no botão "+ Nova Conta" |
| E selecionamos um cliente cadastrado |
| E preenchemos os campos obrigatórios com dados válidos |
| E informamos o título, valor e vencimento |
| QUANDO clicarmos no botão "Salvar" |
| ENTÃO a nova conta deverá ser cadastrada e exibida na listagem |

| Critérios de aceitação |
|---|
| O sistema deve cadastrar a conta corretamente, gerar um código de identificação e vincular o registro ao cliente selecionado. |

| Resultado obtido |
|---|
| Ao preencher todos os campos  a ação foi concluída com sucesso, com resalva do campo de 'tipo de pagamento',
o sistema não aceita algumas opções,  abrindo até uma aba para selecionar a bandeira, para a forma escolhida PIX.|

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
| https://jam.dev/c/61151ba1-c55f-48b3-ac87-6d0af52ad0ea |

---
