# Cenário 14: Gerenciamento de Funções Profissionais

---

## Caso de Teste CT01: Cadastrar função com dados válidos

| ID | Descrição |
|---|---|
| **C14-CT01** | Verificar se o sistema SIFIT permite cadastrar uma nova função profissional utilizando informações válidas. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT e possuir permissão para cadastrar funções profissionais. |

| Passos |
|---|
| DADO que estamos na página de Funções |
| E clicamos no botão "+ Nova Função" |
| E informamos o nome "Instrutor de Musculação" |
| E selecionamos "Interno" no campo "Tipo de Funcionário" |
| E selecionamos "Sim" no campo "Personal" |
| E selecionamos "Não" no campo "Avaliador" |
| QUANDO clicarmos no botão "Salvar Função" |
| ENTÃO o sistema deverá cadastrar a função e apresentá-la na listagem |

| Critérios de aceitação |
|---|
| O sistema deve cadastrar a função corretamente, gerar um código de identificação e preservar o nome, tipo de funcionário e configurações de Personal e Avaliador. |

| Resultado obtido |
|---|
| Cadastrado com Sucesso. |

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
|https://jam.dev/c/1fe41bcb-de08-443c-9c8b-5d4d7bd7b05a |

## Caso de Teste CT02: Cadastrar função com nome vazio

| ID | Descrição |
|---|---|
| **C14-CT02** | Verificar se o sistema impede o cadastro de uma função profissional sem informar seu nome. |

| Pré-condições |
|---|
| O usuário deve estar autenticado e possuir acesso ao cadastro de funções. |

| Passos |
|---|
| DADO que estamos no formulário "Nova Função" |
| E deixamos o campo "Nome" vazio |
| E preenchemos os demais campos disponíveis |
| QUANDO clicarmos no botão "Salvar Função" |
| ENTÃO o sistema deverá impedir o cadastro |

| Critérios de aceitação |
|---|
| O sistema deve exigir o preenchimento do nome e apresentar uma mensagem de validação, sem criar registros com identificação vazia. |

| Resultado obtido |
|---|
| O sistema não deixa cadastrar sem preencher o campo com o nome da função. |

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
| https://jam.dev/c/030fa41b-be71-42e9-8d03-9f72ffb54776|
