# RF09 — Gerenciamento de Matrículas

---

## Caso de Teste CT01: Cadastrar matrícula com dados válidos

| ID | Descrição |
|---|---|
| **C09-CT01** | Verificar se o sistema SIFIT permite cadastrar uma nova matrícula utilizando informações válidas. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT, possuir permissão para cadastrar matrículas e existir um cliente ativo cadastrado no sistema. |

| Passos |
|---|
| DADO que estamos na página "Cadastrar Matrícula" |
| E selecionamos um cliente cadastrado |
| E selecionamos uma modalidade válida |
| E informamos as datas inicial e final |
| E preenchemos os dados de pagamento e os valores da matrícula |
| QUANDO clicarmos no botão "Salvar" |
| ENTÃO o sistema deverá cadastrar a matrícula e vinculá-la ao cliente selecionado |

| Critérios de aceitação |
|---|
| O sistema deve cadastrar a matrícula corretamente, mantendo o vínculo com o cliente, modalidade, período, status e informações financeiras. |

| Resultado obtido |
|---|
|Matrícula cadastrada com sucesso, porém a data de vencimento dá a opção, mas opçao pode ser alterada permanecendo assim fixa pelo sistema dia 25,
o campo taxa da matricula não apresenta formatação R$, com vírgula para centavos, podendo assim ser suscetível a erros de valores digitados.|

| Status |
|---|
|✅ Aprovado. |

| Evidência(s) |
|---|
| https://jam.dev/c/8ddaef45-8448-4c09-a253-6ca807f569ac |
