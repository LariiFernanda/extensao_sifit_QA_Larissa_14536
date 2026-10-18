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
|Os títulos, legendas e informações dos gráficos devem possuir contraste  |   |  Os gráficos são carregados, porém alguns títulos |
|adequado em relação ao fundo, permitindo que o usuário visualize  |           |   e informações aparecem com cores muito próximas às do fundo, |
|e interprete os indicadores gerenciais com facilidade. |                      |  comprometendo a legibilidade e dificultando a interpretação dos dados. |

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

