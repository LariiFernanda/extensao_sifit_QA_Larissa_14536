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
