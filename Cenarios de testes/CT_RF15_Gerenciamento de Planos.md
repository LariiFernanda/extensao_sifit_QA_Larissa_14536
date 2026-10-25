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

## Caso de Teste CT02: Cadastrar plano com campos obrigatórios vazios

| ID | Descrição |
|---|---|
| **C15-CT02** | Verificar se o sistema impede o cadastro de planos sem o preenchimento dos campos obrigatórios. |

| Pré-condições |
|---|
| O usuário deve estar autenticado e possuir permissão para cadastrar planos. |

| Passos |
|---|
| DADO que estamos no formulário "Novo Plano" |
| E deixamos o campo "Nome" vazio |
| E não selecionamos um grupo |
| E deixamos as demais informações obrigatórias sem preenchimento |
| QUANDO clicarmos no botão "Salvar Plano" |
| ENTÃO o sistema deverá impedir o cadastro incompleto |

| Critérios de aceitação |
|---|
| O sistema deve validar os campos obrigatórios, informar quais precisam ser preenchidos e não permitir a criação de planos incompletos. |

| Resultado obtido |
|---|
| O sistema realmente impede que seja cadastrado o plano sem preencher os campos obrigatórios. |

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
| https://jam.dev/c/7d18f69d-2210-413f-b441-a5c1e91cec58 |

---
