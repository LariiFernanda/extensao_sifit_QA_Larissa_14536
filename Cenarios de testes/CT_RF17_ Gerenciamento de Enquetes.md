


## Caso de Teste CT01: Cadastrar nova enquete com dados válidos

| ID | Descrição |
|---|---|
| **RF17-CT01** | Verificar se o sistema SIFIT permite cadastrar uma nova enquete utilizando dados válidos. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT e possuir permissão para cadastrar enquetes. |

| Passos |
|---|
| DADO que estamos na página de Gerenciamento de Enquetes |
| E clicamos no botão "+ Nova Enquete" |
| E preenchemos os campos obrigatórios com informações válidas |
| E adicionamos uma pergunta, caso o cadastro permita |
| QUANDO clicarmos no botão de salvar |
| ENTÃO o sistema deverá cadastrar a nova enquete |
| E apresentar a enquete na listagem |

| Critérios de aceitação |
|---|
| O sistema deve cadastrar a enquete corretamente, gerar um código de identificação e atualizar a quantidade total de enquetes cadastradas. |

| Resultado obtido |
|---|
| Após preencher todos os campos da enquete, o sistema nao permitiu cadastrar a enquete, nao permitiu a digitação por código, não possui a opção de
remover campos de respostas caso o usuário volte atrás mesmo que ainda na edição, e não salvou.|

| Status |
|---|
| Reprovado |

| Evidência(s) |
|---|
Vídeo:
| https://jam.dev/c/9bc9f52b-3124-48da-a7de-cdcfea5ef6d9 |

