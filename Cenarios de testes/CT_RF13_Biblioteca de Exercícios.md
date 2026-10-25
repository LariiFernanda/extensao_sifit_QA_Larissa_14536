# Cenário 13:  Biblioteca de Exercícios

## Caso de Teste CT01: Cadastrar exercício com dados válidos

| ID | Descrição |
|---|---|
| **C13-CT01** | Verificar se o sistema SIFIT permite cadastrar um novo exercício em um grupo muscular. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT e possuir permissão para cadastrar exercícios. Deve existir pelo menos um grupo muscular cadastrado. |

| Passos |
|---|
| DADO que estamos na página Biblioteca de Exercícios |
| E selecionamos o grupo muscular "Bíceps" |
| QUANDO clicarmos no botão "+ Adicionar" |
| E preenchermos os dados obrigatórios do exercício |
| E confirmarmos o cadastro |
| ENTÃO o novo exercício deverá aparecer na lista do grupo "Bíceps" |

| Critérios de aceitação |
|---|
| O sistema deve cadastrar o exercício corretamente, vinculá-lo ao grupo muscular selecionado e atualizar a quantidade de exercícios exibida. |

| Resultado obtido |
|---|
|Resultado positivo, como o esperado, cadastrado com sucesso. |

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
| https://jam.dev/c/cfb01fa2-079e-4ebb-bac9-20ceadafc6df |
