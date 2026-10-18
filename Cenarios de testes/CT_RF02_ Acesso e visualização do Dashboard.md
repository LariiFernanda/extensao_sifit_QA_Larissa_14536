## Cenário 02: Acesso e visualização do Dashboard.

### Caso de Teste 01: Acesso ao Dashboard após login bem-sucedido.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C02-CT01 | Verificar se o sistema SIFIT permite o acesso ao Dashboard após a autenticação bem-sucedida, apresentando corretamente os indicadores e as informações gerenciais da academia. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve possuir uma conta ativa no sistema SIFIT,
com credenciais válidas e permissão para acessar o Dashboard. O sistema deve estar disponível para navegação.     |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que estou na página de login do SIFIT                                            |
| E informo minhas credenciais válidas nos campos "Login" e "Senha"                         |
| **QUANDO** clico no botão "Entrar"                                                        |
| E sou autenticada e direcionada à página inicial do sistema                               |
| E seleciono a opção "Dashboard" no menu lateral                                           |
| **ENTÃO** o sistema deverá apresentar o Dashboard com os indicadores                      |
| e as informações gerenciais da academia, sem apresentar erros de carregamento ou navegação|

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deverá permitir o acesso ao Dashboard após a autenticação do usuário, exibindo corretamente seus componentes visuais, indicadores, gráficos e informações gerenciais disponíveis, sem apresentar falhas de carregamento ou mensagens de erro.     |

**Resultado obtido:**
Durante a execução do teste, realizei o login no sistema SIFIT utilizando credenciais válidas e, após acessar a página inicial, selecionei a opção "Dashboard" no menu lateral.

O sistema permitiu o acesso à página e apresentou os indicadores da seção "Inteligência Sifit", incluindo informações sobre alunos em risco, aniversariantes, avaliações próximas do vencimento e frequência dos alunos.
Também observei o carregamento dos gráficos relacionados aos clientes, como frequência, faixa etária e sexo, além dos gráficos referentes às matrículas.

Status: Aprovado com ressalvas quanto ao acesso e carregamento. Identificada falha visual que deverá ser registrada para correção, pois apresenta inconsistência visual na apresentação das informações. Alguns títulos e textos dos gráficos aparecem com cores muito próximas às do fundo quando no modo CLARO, dificultando a leitura e a identificação dos dados. (Mais Detalhes em Relatórios de Bugs).

**Evidências:**
Print da execução:
<img width="1887" height="927" alt="image" src="https://github.com/user-attachments/assets/5258c48e-022a-46cc-9546-51ca6c89fd5f" />
<img width="1902" height="976" alt="image" src="https://github.com/user-attachments/assets/0f63a271-aa07-4942-b892-692a07437db2" />

Vídeo da execução:
https://jam.dev/c/97986eeb-3c8c-4cfe-bf54-7b1155e95f28

---

### Caso de Teste 02: Verificação da exibição dos widgets do Dashboard.

| ID       | Descrição                                                 |
| :------- | :-------------------------------------------------------- |
| C02-CT02 | Os widgets padrão devem ser exibidos corretamente no Dashboard. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar na tela do Dashboard após login.         |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário está autenticado                          |
| **E** está visualizando o Dashboard                              |
| **QUANDO** a página for carregada                                |
| **ENTÃO** widgets como \"Time at Work\" e \"My Actions\" devem ser exibidos |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Todos os widgets principais devem ser visíveis e funcionais.     |

---

### Caso de Teste 03: Acesso ao Dashboard com sessão expirada.

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C02-CT03 | O sistema deve redirecionar o usuário para o login se a sessão estiver expirada. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário estava logado, mas a sessão expirou.                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessou o sistema anteriormente            |
| **E** permaneceu inativo por um longo período                    |
| **QUANDO** tentar acessar o Dashboard novamente                  |
| **ENTÃO** o sistema deve redirecioná-lo para a página de login    |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A sessão expirada deve ser tratada corretamente com redirecionamento. |
