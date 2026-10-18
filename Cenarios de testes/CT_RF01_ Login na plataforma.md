## Cenário 01: Login na plataforma.

### Caso de Teste 01: Login com as credenciais válidas.

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT01 | Verificar se o sistema SIFIT permite que um usuário cadastrado realize login utilizando credenciais válidas. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve possuir uma conta ativa no sistema SIFIT, com nome de usuário ou e-mail e senha válidos. |

| **Passos**                                                                    |
| :----------------------------------------------------------------             |
| DADO que estamos na página de login do SIFIT                                  |
|E preenchemos o campo de usuário ou e-mail com uma credencial válida           |
|E preenchemos o campo de senha com uma senha válida                            |
|QUANDO clicarmos no botão "Entrar"                                             |
|ENTÃO seremos autenticados e redirecionados para a página inicial do sistema   |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Critérios de aceitação
O sistema deve autenticar o usuário e redirecioná-lo corretamente para a página inicial ou Dashboard,
exibindo as funcionalidades correspondentes ao seu perfil. |
<img width="1151" height="852" alt="image" src="https://github.com/user-attachments/assets/067db1d1-e520-42dc-a49a-fc207c7a6934" />

https://jam.dev/c/979da446-11f1-4c87-8873-af458b1f3d57
---

### Caso de Teste 02: Tentativa de login com senha incorreta.

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT02 | Verificar se o sistema SIFIT impede a autenticação de um usuário quando uma senha incorreta é informada.            |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve possuir uma conta cadastrada no sistema SIFIT e informar uma senha diferente da senha válida de acesso.|

| **Passos**                                                        |
| :---------------------------------------------------------------- |
|DADO que estamos na página de login do SIFIT                             |  
|E preenchemos o campo "Login" com um e-mail cadastrado no sistema        |
|E preenchemos o campo "Senha" com uma senha incorreta                    |
|QUANDO clicarmos no botão "Entrar"                                       |
|ENTÃO o sistema deverá impedir a autenticação e apresentar uma mensagem  |
|informando que as credenciais não correspondem                           |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve impedir o acesso com uma senha incorreta,      |
| permanecer na página de login e exibir uma mensagem de erro   |
| informando que as credenciais fornecidas são inválidas.       |
<img width="775" height="700" alt="image" src="https://github.com/user-attachments/assets/8302e1da-ae6a-4dde-bf10-a514539f8b9f" />
https://jam.dev/c/c5eb0694-fe80-4eed-a02d-90ddfb9b8c68


---

### Caso de Teste 03: Tentativa de login com campos em branco.

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT03 | O login falhará quando os campos obrigatórios estiverem em branco. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Nenhuma. |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que estamos na página de login do OrangeHRM              |
| **E** deixamos os campos de usuário e senha em branco             |
| **QUANDO** clicarmos no botão "Login"                             |
| **ENTÃO** deve ser exibida a mensagem \"Required\" em ambos os campos |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem exibir mensagens de validação.     |
