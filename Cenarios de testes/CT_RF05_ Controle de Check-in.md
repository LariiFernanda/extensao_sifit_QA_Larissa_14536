## Cenário 05: Controle de Check-in

## Caso de Teste 05: Realizar check-in com código válido

| ID | Descrição |
|---|---|
| **RF05-CT01** | Verificar se o sistema SIFIT permite realizar o check-in de um cliente utilizando um código válido. |

| Pré-condições |
|---|
| O usuário deve estar autenticado no SIFIT e possuir permissão para realizar check-ins. O cliente deve estar cadastrado e autorizado a acessar a academia. |

| Passos |
|---|
| DADO que estamos na página de Check-ins do SIFIT |
| E localizamos a seção "Entrada rápida" |
| E informamos um código válido no campo "Código do cliente" |
| QUANDO clicarmos no botão "Realizar check-in" |
| ENTÃO o sistema deverá registrar a entrada do cliente |
| E atualizar a listagem de check-ins |

| Critérios de aceitação |
|---|
| O sistema deve registrar o check-in corretamente, vinculando a entrada ao cliente, à unidade selecionada, à data e ao horário da operação. |

| Resultado obtido |
|---|
| Check-in, realizado com Sucesso. |

| Status |
|---|
| Aprovado. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução:
https://jam.dev/c/1d2e1849-a197-428b-a590-81d7884a3c6c
