# Cenário 15:  Gerenciamento de Planos

---

## Caso de Teste CT01: Cadastrar plano com dados válidos

| ID | Descrição |
|---|---|
| **C15-CT01** | Verificar se o sistema SIFIT permite cadastrar um novo plano utilizando informações válidas. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT e possuir permissão para cadastrar planos. Deve existir pelo menos um grupo disponível para vinculação. |

| Passos |
|---|
| DADO que estamos na página de Planos |
| E clicamos no botão "+ Novo Plano" |
| E informamos o nome "Plano Mensal de Musculação" |
| E selecionamos um grupo cadastrado |
| E definimos o status como "Ativo" |
| E selecionamos "Mensalidade recorrente" no campo "Cobrança" |
| E preenchemos os valores e demais informações obrigatórias |
| QUANDO clicarmos no botão "Salvar Plano" |
| ENTÃO o sistema deverá cadastrar o novo plano |

| Critérios de aceitação |
|---|
| O sistema deve cadastrar o plano corretamente, gerar um código identificador e preservar suas configurações financeiras e operacionais. |

| Resultado obtido |
|---|
| Cadastrado com Sucesso.|

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
|https://jam.dev/c/2693311a-555a-4f18-90da-cd299ce0607b |
