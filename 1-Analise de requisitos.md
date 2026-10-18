# 📦 Requisitos Funcionais Detalhados para Testes Manuais — SIFIT

## 🏋️ Visão Geral

O **SIFIT — Sistema de Gestão de Academias** é uma plataforma voltada à administração de academias, reunindo funcionalidades relacionadas à gestão de clientes, matrículas, avaliações físicas, controle de frequência, treinamentos, finanças e automações.

Este documento apresenta os requisitos funcionais utilizados como referência para o planejamento e a execução dos testes manuais de Qualidade de Software (QA).

Os requisitos foram elaborados a partir da análise das telas disponíveis no sistema, com o objetivo de identificar os comportamentos esperados, avaliar as funcionalidades e documentar possíveis inconsistências.

> **Nota:** os requisitos apresentados representam uma especificação preliminar baseada nas interfaces observadas. As regras de negócio ainda deverão ser verificadas durante os testes e, quando possível, confirmadas com a documentação oficial do SIFIT.

---

## 🔐 RF01 — Autenticação e Controle de Acesso

**Descrição:** O sistema deve permitir que usuários cadastrados realizem a autenticação e acessem as funcionalidades disponíveis conforme suas permissões.

**Funcionalidades esperadas:**
- Realizar login utilizando credenciais válidas.
- Impedir o acesso com login ou senha incorretos.
- Validar os campos obrigatórios de autenticação.
- Exibir mensagens claras quando ocorrer falha no login.
- Disponibilizar a opção "Esqueci minha senha".
- Permitir a utilização da opção "Manter conectado".
- Disponibilizar mecanismos para encerramento da sessão.
- Restringir o acesso às funcionalidades administrativas para usuários não autorizados.

**Pontos de validação QA:**
- Login com credenciais válidas e inválidas.
- Login com campos vazios.
- Recuperação de senha.
- Persistência da sessão e encerramento do acesso.
- Tentativa de acessar páginas restritas sem autenticação.

---

## 🏠 RF02 — Página Inicial e Dashboard Gerencial

**Descrição:** Após a autenticação, o sistema deve disponibilizar informações administrativas e indicadores relacionados ao funcionamento da academia.

**Funcionalidades esperadas:**
- Apresentar a página inicial com resumo das informações da academia.
- Disponibilizar navegação para o Dashboard por meio do menu lateral.
- Exibir indicadores de clientes ativos, ausentes e sem matrículas.
- Apresentar informações sobre matrículas, renovações e desistências.
- Exibir mensalidades pendentes e valores financeiros.
- Apresentar gráficos de frequência, faixa etária, sexo e matrículas.
- Disponibilizar indicadores de retenção e risco de evasão.
- Permitir a visualização de notificações e informações da agenda.
- Apresentar os dados de maneira clara e legível.

**Pontos de validação QA:**
- Acesso ao Dashboard após autenticação.
- Carregamento dos indicadores e gráficos.
- Navegação entre Página Inicial e Dashboard.
- Legibilidade dos títulos e informações.
- Consistência dos valores apresentados.
- Funcionamento dos atalhos e filtros disponíveis.

---

## 👥 RF03 — Gerenciamento de Clientes

**Descrição:** O sistema deve permitir o gerenciamento das informações cadastrais dos clientes da academia.

**Funcionalidades esperadas:**
- Cadastrar novos clientes.
- Listar e consultar clientes cadastrados.
- Pesquisar clientes por código ou nome.
- Filtrar clientes por status, situação financeira, plano e personal.
- Consultar informações individuais dos clientes.
- Permitir edição dos dados cadastrais.
- Disponibilizar ações de exclusão ou desativação, conforme as regras do sistema.
- Apresentar indicadores de clientes cadastrados, ativos, ausentes e sem matrícula.

**Pontos de validação QA:**
- Cadastro com informações válidas.
- Cadastro com campos obrigatórios vazios.
- Pesquisa por código e nome.
- Funcionamento dos filtros combinados.
- Alteração de informações cadastrais.
- Exclusão ou desativação de registros.
- Atualização dos indicadores após modificações.

---

## 📝 RF04 — Gerenciamento de Matrículas

**Descrição:** O sistema deve permitir o cadastro e o acompanhamento das matrículas dos alunos, incluindo informações contratuais e financeiras.

**Funcionalidades esperadas:**
- Cadastrar novas matrículas vinculadas aos clientes.
- Identificar o funcionário responsável pelo cadastro.
- Registrar data de início e término da matrícula.
- Selecionar modalidade e situação da matrícula.
- Informar se a matrícula é uma renovação.
- Definir moeda e tipo de pagamento.
- Registrar taxa de matrícula, valor da parcela e descontos.
- Apresentar o valor total da matrícula.
- Definir o dia de vencimento.
- Disponibilizar campo de observações.
- Permitir consulta e gerenciamento das matrículas existentes.

**Pontos de validação QA:**
- Cadastro de matrícula com dados válidos.
- Tentativa de cadastro sem selecionar um aluno.
- Validação de datas de início e término.
- Cadastro com valores negativos ou inválidos.
- Cálculo de descontos e valor total.
- Associação da matrícula ao cliente correto.
- Persistência dos dados após salvar.

---

## 🏋️ RF05 — Avaliações Físicas

**Descrição:** O sistema deve permitir o registro e o acompanhamento de avaliações físicas dos alunos.

**Funcionalidades esperadas:**
- Cadastrar novas avaliações físicas.
- Consultar avaliações existentes.
- Pesquisar registros por código ou nome.
- Filtrar avaliações por status.
- Associar avaliações a alunos e profissionais.
- Apresentar data e horário da avaliação.
- Identificar avaliações pendentes e realizadas.
- Disponibilizar ações de visualização, edição ou exclusão conforme o status.
- Apresentar indicadores de avaliações realizadas no mês e períodos anteriores.

**Pontos de validação QA:**
- Cadastro de avaliação com dados válidos.
- Busca por cliente ou código.
- Filtragem por status.
- Alteração de uma avaliação pendente.
- Validação dos dados obrigatórios.
- Verificação da atualização dos indicadores.
- Funcionamento das ações disponíveis para cada registro.

---

## ⏱️ RF06 — Controle de Check-in

**Descrição:** O sistema deve permitir o registro e o acompanhamento das entradas dos alunos na academia.

**Funcionalidades esperadas:**
- Realizar check-in manual.
- Identificar alunos por código ou leitura de QR Code.
- Pesquisar registros por nome, código ou plano.
- Filtrar check-ins por situação.
- Apresentar a quantidade de check-ins realizados no dia.
- Exibir alunos presentes em tempo real.
- Disponibilizar informações sobre horários de entrada e saída.
- Apresentar indicadores de frequência e movimentação.
- Permitir selecionar a unidade da academia.

**Pontos de validação QA:**
- Check-in com código válido.
- Check-in com código inexistente.
- Tentativa de registro duplicado.
- Check-in de aluno sem matrícula válida.
- Atualização da quantidade de presentes.
- Funcionamento dos filtros e pesquisas.

---

## 📅 RF07 — Histórico de Presenças

**Descrição:** O sistema deve permitir consultar os registros de frequência dos alunos em períodos específicos.

**Funcionalidades esperadas:**
- Pesquisar presenças por cliente.
- Consultar registros por intervalo de datas.
- Disponibilizar filtros rápidos para hoje, semana e mês.
- Apresentar o total de presenças no período.
- Exibir a quantidade de alunos distintos.
- Calcular a média diária de presenças.
- Informar a quantidade de dias considerados na consulta.
- Apresentar mensagens quando não houver registros.

**Pontos de validação QA:**
- Consulta por períodos diferentes.
- Pesquisa por nome do aluno.
- Validação de datas inválidas.
- Consistência dos indicadores de frequência.
- Tratamento de períodos sem resultados.

---

## 📚 RF08 — Fichas de Treino

**Descrição:** O sistema deve permitir cadastrar e organizar fichas de treinamento vinculadas aos alunos e profissionais responsáveis.

**Funcionalidades esperadas:**
- Cadastrar novas fichas de treino.
- Identificar o funcionário responsável pelo cadastro.
- Selecionar o aluno por código ou nome.
- Associar um personal à ficha.
- Definir datas de início e término.
- Selecionar o objetivo do treinamento.
- Registrar observações adicionais.
- Disponibilizar criação de ficha personalizada.
- Permitir utilizar modelos de fichas.
- Consultar fichas cadastradas e seus status.

**Pontos de validação QA:**
- Cadastro de ficha com informações válidas.
- Tentativa de cadastro sem aluno.
- Validação das datas do treinamento.
- Associação da ficha ao personal correto.
- Utilização de modelos disponíveis.
- Consulta e acompanhamento dos registros.

---

## 💪 RF09 — Biblioteca de Exercícios e Grupos Musculares

**Descrição:** O sistema deve permitir organizar exercícios físicos em grupos musculares, facilitando a elaboração dos treinamentos.

**Funcionalidades esperadas:**
- Listar os grupos musculares cadastrados.
- Classificar grupos por tipo de membro corporal.
- Cadastrar novos grupos musculares.
- Consultar, editar e excluir grupos existentes.
- Organizar exercícios por grupo muscular.
- Adicionar exercícios à biblioteca.
- Consultar e excluir exercícios cadastrados.
- Apresentar a quantidade de exercícios por grupo.

**Pontos de validação QA:**
- Cadastro de novos exercícios.
- Cadastro de grupos musculares.
- Validação de nomes duplicados.
- Associação de exercícios aos grupos corretos.
- Exclusão de exercícios e grupos.
- Atualização dos totais apresentados.

---

## 🗓️ RF10 — Gerenciamento de Turmas e Modalidades

**Descrição:** O sistema deve permitir cadastrar, organizar e acompanhar turmas e modalidades oferecidas pela academia.

**Funcionalidades esperadas:**
- Cadastrar novas turmas.
- Pesquisar turmas por código ou nome.
- Filtrar turmas por status.
- Associar turmas aos planos ou modalidades.
- Definir horários de início e término.
- Selecionar os dias da semana.
- Associar profissionais responsáveis.
- Definir a quantidade de vagas quando disponível.
- Consultar, editar e excluir turmas.
- Apresentar indicadores de turmas cadastradas, ativas e experimentais.

**Pontos de validação QA:**
- Cadastro com dados válidos.
- Validação dos horários.
- Tentativa de cadastro sem dias definidos.
- Definição de quantidade de vagas.
- Edição de turma existente.
- Funcionamento dos filtros de pesquisa.
- Verificação das regras para horários conflitantes.

---

## 🏃 RF11 — SifitBox e Categorias CrossFit

**Descrição:** O sistema deve disponibilizar recursos para organização das aulas e categorias relacionadas às modalidades de treinamento funcional e CrossFit.

**Funcionalidades esperadas:**
- Consultar aulas por período.
- Disponibilizar a opção de gerar aulas.
- Cadastrar e gerenciar modalidades.
- Organizar turmas recorrentes.
- Definir dias, horários e capacidade das turmas.
- Cadastrar categorias CrossFit.
- Pesquisar categorias por código ou nome.
- Editar e excluir categorias existentes.
- Registrar informações de criação e atualização das categorias.

**Pontos de validação QA:**
- Consulta de aulas por intervalo de datas.
- Geração de aulas.
- Cadastro e edição de modalidades.
- Validação dos dados de turmas recorrentes.
- Cadastro de categorias CrossFit.
- Pesquisa e exclusão de categorias.
- Verificação de nomes duplicados.

---

## 💰 RF12 — Contas a Receber

**Descrição:** O sistema deve permitir o controle das receitas e dos valores a receber relacionados às operações da academia.

**Funcionalidades esperadas:**
- Cadastrar novas contas a receber.
- Consultar lançamentos existentes.
- Pesquisar contas por código ou nome do cliente.
- Filtrar registros por data de vencimento e status.
- Disponibilizar filtros rápidos por período.
- Apresentar valores de entradas, saídas e saldo líquido.
- Exibir valores previstos e recebidos no mês.
- Apresentar a quantidade de contas pendentes ou atrasadas.
- Disponibilizar informações de valor recebido e situação de pagamento.

**Pontos de validação QA:**
- Cadastro de conta com dados válidos.
- Registro de recebimentos.
- Pesquisa e filtros por período.
- Validação de valores monetários.
- Atualização dos indicadores financeiros.
- Consistência entre valor previsto, recebido e pendente.

---

## 🧾 RF13 — Contas a Pagar

**Descrição:** O sistema deve permitir o gerenciamento das despesas e obrigações financeiras da academia.

**Funcionalidades esperadas:**
- Cadastrar novas contas a pagar.
- Associar contas a fornecedores ou colaboradores.
- Consultar lançamentos existentes.
- Pesquisar por código ou nome.
- Filtrar contas por data e status.
- Apresentar valores a pagar e valores restantes.
- Identificar contas pendentes e atrasadas.
- Permitir consulta e exclusão conforme as permissões do usuário.
- Disponibilizar paginação dos registros.

**Pontos de validação QA:**
- Cadastro de nova despesa.
- Validação de campos obrigatórios.
- Cadastro com valores inválidos.
- Pesquisa por fornecedor.
- Alteração da situação de pagamento.
- Consistência dos indicadores.
- Funcionamento da paginação.

---

## 🏢 RF14 — Gerenciamento de Fornecedores

**Descrição:** O sistema deve permitir o cadastro e a manutenção dos fornecedores vinculados às atividades da academia.

**Funcionalidades esperadas:**
- Cadastrar novos fornecedores.
- Listar fornecedores cadastrados.
- Pesquisar por código ou nome.
- Consultar dados dos fornecedores.
- Permitir edição e exclusão conforme as regras do sistema.
- Identificar fornecedores ativos e inativos.
- Apresentar indicadores de fornecedores cadastrados e ativos.

**Pontos de validação QA:**
- Cadastro com informações válidas.
- Cadastro com campos obrigatórios vazios.
- Pesquisa por código e nome.
- Consulta e atualização dos registros.
- Verificação de fornecedores duplicados.
- Atualização dos indicadores.

---

## 👨‍🏫 RF15 — Gerenciamento de Funções Profissionais

**Descrição:** O sistema deve permitir organizar as funções exercidas pelos profissionais vinculados à academia.

**Funcionalidades esperadas:**
- Cadastrar novas funções.
- Pesquisar funções por código ou nome.
- Filtrar funções por tipo.
- Classificar funções como internas ou externas.
- Identificar funções relacionadas à atuação como personal.
- Identificar funções relacionadas à realização de avaliações físicas.
- Consultar as informações de cada função.
- Disponibilizar indicadores das funções cadastradas.

**Pontos de validação QA:**
- Cadastro de função.
- Validação de campos obrigatórios.
- Pesquisa e filtros.
- Classificação entre interno e externo.
- Definição das atribuições de personal e avaliador.
- Consulta e atualização dos registros.

---

## 📄 RF16 — Tipos de Documentos

**Descrição:** O sistema deve permitir organizar os tipos de documentos utilizados nos cadastros administrativos da academia.

**Funcionalidades esperadas:**
- Cadastrar novos tipos de documentos.
- Pesquisar documentos por código ou nome.
- Classificar a aplicação dos documentos.
- Associar tipos de documentos a fornecedores ou colaboradores.
- Consultar os documentos cadastrados.
- Disponibilizar ações de gerenciamento.
- Apresentar indicadores por categoria de aplicação.

**Pontos de validação QA:**
- Cadastro de novo tipo de documento.
- Validação do nome e da aplicação.
- Pesquisa por código e nome.
- Funcionamento dos filtros.
- Exclusão de registros.
- Atualização das quantidades apresentadas.

---

## 📋 RF17 — Gerenciamento de Enquetes

**Descrição:** O sistema deve permitir cadastrar, organizar e acompanhar enquetes utilizadas para coleta de informações e opiniões.

**Funcionalidades esperadas:**
- Cadastrar novas enquetes.
- Consultar enquetes existentes.
- Pesquisar por código ou nome.
- Filtrar enquetes por status.
- Identificar enquetes ativas e inativas.
- Apresentar as perguntas cadastradas.
- Disponibilizar a quantidade de respostas recebidas.
- Permitir gerenciar os registros conforme as permissões disponíveis.

**Pontos de validação QA:**
- Cadastro de enquete com informações válidas.
- Tentativa de ativar enquete sem perguntas.
- Pesquisa e filtros por status.
- Validação dos campos obrigatórios.
- Verificação da contagem de respostas.
- Exclusão ou desativação de enquetes.

---

## 🤖 RF18 — Inteligência e Automação

**Descrição:** O sistema deve disponibilizar recursos de automação para auxiliar na gestão da academia e no acompanhamento dos alunos.

**Funcionalidades esperadas:**
- Apresentar as automações ativas.
- Permitir ativar ou desativar automações disponíveis.
- Disponibilizar a execução manual de automações.
- Apresentar informações sobre a última execução.
- Registrar o histórico das atividades realizadas.
- Monitorar indicadores relacionados ao risco de evasão.
- Disponibilizar automações relacionadas a aniversariantes.
- Utilizar canais de comunicação configurados, como WhatsApp.
- Permitir consultar resultados das automações executadas.
- Identificar recursos ainda em desenvolvimento.

**Pontos de validação QA:**
- Ativação e desativação de automações.
- Execução manual.
- Atualização da data de última execução.
- Visualização do histórico.
- Consistência dos indicadores de retenção.
- Tratamento de falhas nas execuções.
- Verificação da disponibilidade dos recursos sinalizados como em desenvolvimento.

---

## 📌 Critérios Gerais para os Testes Manuais

Durante a execução dos casos de teste, deverão ser considerados os seguintes aspectos:

| Critério | Descrição |
|---|---|
| **Funcionalidade** | Verificar se a operação atende ao comportamento esperado. |
| **Validação** | Avaliar o tratamento de dados obrigatórios, inválidos ou incompletos. |
| **Navegação** | Verificar o acesso e o redirecionamento entre as funcionalidades. |
| **Persistência** | Confirmar se os dados salvos permanecem registrados corretamente. |
| **Consistência** | Comparar os indicadores com os registros apresentados e, quando necessário, com o banco de dados. |
| **Usabilidade** | Avaliar a organização, clareza e legibilidade das informações. |
| **Segurança** | Verificar se as funcionalidades respeitam os controles de acesso previstos. |
| **Tratamento de erros** | Avaliar se o sistema apresenta mensagens adequadas diante de situações inesperadas. |

---

## 📈 Resultados Esperados

A execução dos testes manuais busca avaliar a qualidade das funcionalidades do SIFIT, identificando comportamentos que possam comprometer a experiência dos usuários e a confiabilidade das informações.

Os resultados serão documentados por meio de casos de teste, relatórios de bugs e evidências, permitindo acompanhar os cenários aprovados, reprovados ou bloqueados.

A análise também poderá contribuir para identificar oportunidades de melhoria na navegação, nas validações, na apresentação dos dados e nas operações administrativas da academia.

---

## 👩‍💻 Considerações Finais

A documentação dos requisitos funcionais representa uma etapa importante do planejamento dos testes de QA do SIFIT.

Por meio da análise das interfaces e da execução dos cenários, será possível compreender o comportamento das funcionalidades, avaliar sua aderência aos resultados esperados e registrar possíveis inconsistências.

O objetivo não é apenas identificar erros, mas também desenvolver uma visão crítica sobre a qualidade do software, considerando aspectos técnicos, funcionais e relacionados à experiência do usuário.

**Status da documentação:** Em elaboração e validação, conforme a evolução dos testes manuais.
