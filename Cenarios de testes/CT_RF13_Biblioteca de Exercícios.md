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

## Caso de Teste CT02: Cadastrar exercício com campos obrigatórios vazios

| ID | Descrição |
|---|---|
| **C13-CT02** | Verificar se o sistema impede o cadastro de um exercício sem o preenchimento dos campos obrigatórios. |

| Pré-condições |
|---|
| O usuário deve estar autenticado e possuir permissão para cadastrar exercícios. |

| Passos |
|---|
| DADO que estamos na página Biblioteca de Exercícios |
| E clicamos no botão "+ Adicionar" de um grupo muscular |
| E deixamos os campos obrigatórios em branco |
| QUANDO tentarmos salvar o exercício |
| ENTÃO o sistema deverá impedir o cadastro |

| Critérios de aceitação |
|---|
| O sistema deve apresentar mensagens de validação indicando os campos obrigatórios e impedir a criação de registros incompletos. |

| Resultado obtido |
|---|
| Mensagem de validação apresentada com sucesso, e exercício não cadastrado.  |

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
| https://jam.dev/c/17a97d55-fbb5-4b27-b6b5-c8ee5ce8f1b6 |
