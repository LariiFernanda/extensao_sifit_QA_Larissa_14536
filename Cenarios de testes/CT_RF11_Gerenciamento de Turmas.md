# Cenário 11: Gerenciamento de Turmas e Modalidades

---

## Caso de Teste CT01: Cadastrar turma com dados válidos

| ID | Descrição |
|---|---|
| **C11-CT01** | Verificar se o sistema SIFIT permite cadastrar uma nova turma utilizando informações válidas. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT e possuir permissão para cadastrar turmas. Deve existir pelo menos um plano ou modalidade disponível para vinculação. |

| Passos |
|---|
| DADO que estamos na página de Turmas |
| E clicamos no botão "Cadastrar Turma" |
| E informamos um nome válido para a turma |
| E selecionamos um plano ou modalidade disponível |
| E definimos o horário inicial e final |
| E selecionamos os dias da semana |
| E preenchemos os demais campos obrigatórios |
| QUANDO clicarmos no botão "Salvar" |
| ENTÃO o sistema deverá cadastrar a turma e exibi-la na listagem |

| Critérios de aceitação |
|---|
| O sistema deve cadastrar a turma corretamente, gerar um código de identificação e manter as informações de nome, plano, horários, dias e status vinculadas ao registro. |

| Resultado obtido |
|---|
| Ao preencher todos os campos o resultado foi como o esperado, realizado com sucesso. |

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
|https://jam.dev/c/54a7f12a-70af-4b27-80dd-987bc31689ce|


## Caso de Teste CT02: Cadastrar turma com campos obrigatórios vazios

| ID | Descrição |
|---|---|
| **C11-CT02** | Verificar se o sistema impede o cadastro de uma turma sem o preenchimento dos campos obrigatórios. |

| Pré-condições |
|---|
| O usuário deve estar autenticado e possuir permissão para cadastrar turmas. |

| Passos |
|---|
| DADO que estamos na página de Turmas |
| E clicamos no botão "Cadastrar Turma" |
| E deixamos os campos obrigatórios em branco |
| QUANDO tentarmos salvar a turma |
| ENTÃO o sistema deverá validar os campos obrigatórios |
| E impedir o cadastro incompleto |

| Critérios de aceitação |
|---|
| O sistema deve apresentar mensagens de validação indicando os campos obrigatórios e não permitir o cadastro de turmas com informações essenciais ausentes. |

| Resultado obtido |
|---|
| Ao tentar salvar sem preencher os campos, o sistema não deixou salvar, informando uma mensagem de validação para preencher os campos obrigatórios |

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
|https://jam.dev/c/e65a0feb-f064-467d-9ff7-05f737b458e4 |

