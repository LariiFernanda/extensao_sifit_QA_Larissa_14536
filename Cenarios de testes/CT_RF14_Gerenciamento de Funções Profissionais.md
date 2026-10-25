# Cenário 14: Gerenciamento de Funções Profissionais

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

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
