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
O sistema deve autenticar o usuário e redirecioná-lo corretamente para a página inicial ou Dashboard,
exibindo as funcionalidades correspondentes ao seu perfil. |

Resultado obtido: O sistema realizou a autenticação do usuário com credenciais válidas e efetuou o redirecionamento para a página inicial, conforme o comportamento esperado.

Status: Aprovado.

**Evidências:**
Print da execução: 
<img width="1151" height="852" alt="image" src="https://github.com/user-attachments/assets/067db1d1-e520-42dc-a49a-fc207c7a6934" />
<img width="1907" height="912" alt="image" src="https://github.com/user-attachments/assets/3d1e142a-d2d9-430d-8340-37bc2dcbd393" />

|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução:
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

Resultado obtido: Ao realizar uma tentativa de login com senha incorreta, o sistema SIFIT impediu a autenticação e exibiu a mensagem "O nome de usuário e senha não correspondem.", permanecendo na página de login.

Status: Aprovado.

**Evidências:**
Print da execução: 
<img width="775" height="700" alt="image" src="https://github.com/user-attachments/assets/8302e1da-ae6a-4dde-bf10-a514539f8b9f" />


|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução:
https://jam.dev/c/c5eb0694-fe80-4eed-a02d-90ddfb9b8c68


---

### Caso de Teste 03: Tentativa de login com campos em branco.

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT03 | Verificar se o sistema SIFIT impede a autenticação quando os campos obrigatórios de login e senha não são preenchidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar na página de login do sistema SIFIT, com os campos "Login" e "Senha" em branco.|

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| DADO que estamos na página de login do SIFIT                             | 
| E deixamos o campo "Login" em branco                                     | 
| E deixamos o campo "Senha" em branco                                     | 
| QUANDO clicarmos no botão "Entrar"                                       | 
| ENTÃO o sistema deverá impedir a autenticação e apresentar uma mensagem  | 
| informando que os campos obrigatórios precisam ser preenchidos           | 

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem exibir mensagens de validação.     |

Durante a execução do teste, acessei a página de login do SIFIT e deixei os campos "Login" e "Senha" em branco. Em seguida, cliquei no botão "Entrar" para verificar como o sistema reagiria à ausência das informações obrigatórias.

O sistema impediu o acesso, porém apresentou a mensagem "O nome de usuário e senha não correspondem.", mesmo sem nenhuma credencial ter sido informada.

Como usuária, percebi que essa mensagem pode causar confusão, pois indica que os dados inseridos estão incorretos, quando, na realidade, os campos não foram preenchidos.

Embora o sistema tenha impedido corretamente a autenticação, identifiquei uma falha na comunicação da validação. O comportamento mais adequado seria apresentar uma mensagem específica, como "Preencha os campos de login e senha", orientando o usuário sobre como proceder.

Status: Reprovado — falha na mensagem de validação dos campos obrigatórios.

**Evidências:**
Print da execução: 
<img width="781" height="727" alt="image" src="https://github.com/user-attachments/assets/432f64b7-af94-4807-a4ee-883e9d7becab" />

