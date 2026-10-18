# Relatório de Bugs

**Software:** SIFIT

**QA responsável:**  Larissa Fernanda

**Data:** 18/10/2026 

---

### 🐞 **Bug 01: Baixo contraste nos títulos e informações dos gráficos do Dashboard**

| **ID**     | **Descrição**                                                                                                                                             |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BUG-001    | Ao acessar o Dashboard do SIFIT, alguns títulos e textos dos gráficos apresentam cores muito próximas às do fundo, dificultando a leitura e a interpretação das informações gerenciais da academia.|

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Média         |            Média           |   Aberto   |

| **Passo a passo para simular o bug**                           |
| -------------------------------------------------------------- |
| 1. Acessar a página de login do SIFIT.                                   |
| 2. Informar credenciais válidas e realizar a autenticação.                         |
| 3. Na página inicial, localizar o menu lateral.                              |
| 4. Clicar na opção "Dashboard".                            |
| 5. Observar os títulos e as informações apresentados nos gráficos de clientes e matrículas. |
| 6. Identificar os textos com baixo contraste em relação ao fundo dos gráficos. |

|                        **Comportamento Esperado**                       |                        **Comportamento Obtido**                        |
| :---------------------------------------------------------------------: | :--------------------------------------------------------------------: |
|Os títulos, legendas e informações dos gráficos devem possuir contraste  |     Os gráficos são carregados, porém alguns títulos |
|adequado em relação ao fundo, permitindo que o usuário visualize  |            e informações aparecem com cores muito próximas às do fundo, |
|e interprete os indicadores gerenciais com facilidade. |                       comprometendo a legibilidade e dificultando a interpretação dos dados. |

| **Ambiente**             |
| ------------------------ |
| Ambiente    /     Informações|
|Sistema	         -   SIFIT —  Gestão de Academias|
|Ambient         -   Sistema web|
|Dispositivo     -   Desktop|
|Página afetada  -   Dashboard           |

| **Funcionalidade Afetada** |        **Caso de Teste Relacionado**       |
| :------------------------: | :----------------------------------------: |
| Dashboard / Visualização de indicadores e gráficos | C02-CT01: Acesso ao Dashboard após login bem-sucedido |

|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução:
https://jam.dev/c/97986eeb-3c8c-4cfe-bf54-7b1155e95f28





### 🐞  **Bug 02: Erro interno do servidor durante a navegação no SIFIT**

| **ID**     | **Descrição**                                                                                                                                             |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BUG-002    | Durante a utilização do SIFIT, após um período prolongado de autenticação, o sistema apresenta a mensagem "Erro no servidor — Erro interno inesperado." ao acessar ou utilizar diferentes funcionalidades, prejudicando a navegação e a execução das operações.|

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|    Alta (provisória)  |     Alta (provisória)      |   Aberto   |



|                        **Comportamento Esperado**                       |                        **Comportamento Obtido**                        |
| :---------------------------------------------------------------------: | :--------------------------------------------------------------------: |
|  O sistema deve permitir a navegação entre os módulos enquanto          |     Durante a navegação, o sistema apresenta uma mensagem|
|  a sessão estiver válida.Caso a sessão expire,                          |     genérica de erro interno, sem explicar a causa ou orientar o|
|  deve informar o usuário e solicitar uma nova autenticação.             |     usuário sobre como proceder.                                

Durante a execução dos testes manuais no SIFIT, permaneci autenticada no sistema por mais de uma hora, realizando a navegação entre diferentes funcionalidades.
Nesse período, observei a ocorrência da mensagem "Erro no servidor — Erro interno inesperado.", não sendo um problema limitado à funcionalidade de Check-in.

Como usuária, percebi que a mensagem apresentada não esclarece o motivo da falha e não oferece orientações para solucionar o problema.

Considero importante verificar se o comportamento possui relação com o tempo de duração da sessão ou com alguma falha de comunicação com o servidor, pois esse tipo de ocorrência pode comprometer a utilização contínua da plataforma.

**Sugestão de melhoria:** investigar o gerenciamento das sessões e o tratamento dos erros internos, garantindo que o sistema apresente mensagens claras e permita ao usuário recuperar a navegação de maneira adequada.

|                **Evidência(s)**               |
| :-------------------------------------------: |
Print da execução:
<img width="1917" height="896" alt="image" src="https://github.com/user-attachments/assets/bc050f1e-7a9a-4a6a-ae4f-b5e1ebfd4ee9" />


|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução:
https://jam.dev/c/f57b5c39-dcf1-49ec-bdda-a0b42f85d11a


