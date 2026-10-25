# 🧪 Plano de Testes Manuais — SIFIT

**Sistema de Gestão de Academias | Quality Assurance (QA)**

Este documento apresenta o planejamento dos testes manuais realizados no **SIFIT**, contemplando os objetivos, escopo, metodologia, critérios de aceitação, riscos e entregáveis do processo de avaliação da qualidade do software.

---

## 📌 1. Identificação do Projeto

| Informação | Descrição |
|---|---|
| **Nome do Projeto** | SIFIT — Sistema de Gestão de Academias |
| **Sistema Avaliado** | Plataforma web de gerenciamento de academias |
| **Versão Avaliada** | Versão web disponível durante o período dos testes |
| **Ambiente de Testes** | [SIFIT — Plataforma Web](https://sifit.centrion.com.br/) |
| **Tipo de Teste** | Testes Manuais Funcionais e Exploratórios |
| **Período de Avaliação** | Outubro de 2026 |
| **Responsável** | Larissa — Testadora QA |
| **Finalidade** | Projeto acadêmico de Qualidade de Software |

---

## 🎯 2. Objetivo

O plano de testes tem como objetivo avaliar manualmente as principais funcionalidades do **SIFIT — Sistema de Gestão de Academias**, verificando se os recursos disponíveis apresentam comportamentos adequados às necessidades administrativas e operacionais de uma academia.

A avaliação busca identificar falhas funcionais, problemas de validação, inconsistências na apresentação de informações e dificuldades de navegação que possam comprometer a experiência dos usuários.

**Objetivos específicos:**

- Validar os fluxos de autenticação e acesso às funcionalidades.
- Verificar o comportamento dos formulários e das operações de cadastro.
- Avaliar a navegação entre os módulos administrativos.
- Analisar a apresentação dos indicadores gerenciais e financeiros.
- Identificar inconsistências nas mensagens de validação e tratamento de erros.
- Verificar a consulta, atualização e persistência dos dados quando aplicável.
- Registrar evidências e documentar os defeitos identificados.
- Propor melhorias para os problemas observados durante os testes.

---


---

## 🔧 3. Ferramentas Utilizadas

| Ferramenta | Finalidade |
|---|---|
| **Google Chrome** | Navegação e execução dos testes manuais |
| **Chrome DevTools** | Inspeção de elementos e análise de erros, quando necessário |
| **MySQL Workbench** | Consulta e verificação de informações no banco de dados |
| **MariaDB** | Banco de dados utilizado pelo SIFIT |
| **Jam.dev** | Gravação de testes e documentação visual dos bugs |
| **Captura de Tela** | Registro de evidências dos comportamentos observados |
| **GitHub** | Organização, versionamento e publicação da documentação |
| **Markdown** | Elaboração dos casos de teste e relatórios |

---

## 🧪 4. Técnicas de Teste

Os testes serão executados manualmente, utilizando técnicas adequadas à validação das funcionalidades e à identificação de inconsistências.

| Técnica | Aplicação no SIFIT |
|---|---|
| **Testes positivos** | Verificar o funcionamento das operações com informações válidas. |
| **Testes negativos** | Avaliar a resposta do sistema a dados inválidos ou incompletos. |
| **Particionamento de equivalência** | Organizar entradas em grupos válidos e inválidos para reduzir testes repetitivos. |
| **Análise de valor limite** | Testar limites de datas, valores monetários, quantidades e campos numéricos. |
| **Caminho feliz (Happy Path)** | Verificar a conclusão de processos nas condições esperadas. |
| **Testes exploratórios** | Investigar comportamentos inesperados durante a navegação. |
| **Testes de usabilidade** | Avaliar mensagens, legibilidade, organização visual e facilidade de utilização. |

### Padrão de execução — BDD

Os casos de teste serão descritos utilizando a estrutura:

> **DADO** que estou em determinada página ou condição inicial.
>
> **E** informo os dados necessários para a operação.
>
> **QUANDO** realizo uma ação no sistema.
>
> **ENTÃO** o sistema deverá apresentar o comportamento esperado.

Cada execução será acompanhada de um registro do resultado observado e, sempre que possível, de evidências em imagem ou vídeo.

---

## 📄 5. Critérios de Aceitação

Um caso de teste será considerado aprovado quando o comportamento observado corresponder ao resultado esperado e atender aos requisitos definidos para a funcionalidade.

**Critérios considerados:**

- A funcionalidade executa corretamente a operação solicitada.
- Os campos obrigatórios são validados adequadamente.
- Dados inválidos são tratados sem comprometer o funcionamento do sistema.
- As mensagens de erro são claras e orientam o usuário.
- A navegação ocorre sem redirecionamentos inesperados.
- As informações apresentadas são consistentes com os registros existentes.
- Os componentes da interface apresentam legibilidade adequada.
- As operações de cadastro e atualização são persistidas corretamente, quando aplicável.
- O acesso às funcionalidades respeita as permissões previstas.

### Classificação dos resultados

| Status | Descrição |
|---|---|
| ✅ **Aprovado** | O sistema apresentou o comportamento esperado. |
| ❌ **Reprovado** | Foi identificada uma falha que impede o atendimento de um ou mais critérios de aceitação. |
| 🚫 **Bloqueado** | Não foi possível concluir o teste devido a uma condição impeditiva. |
| ⏳ **Não executado** | O caso de teste ainda não foi realizado. |

Quando uma funcionalidade operar corretamente, mas apresentar uma falha secundária, a inconsistência será registrada e o status do caso será definido conforme os critérios afetados.

---

## 🚦 6. Critérios de Saída (Exit Criteria)

A etapa de testes poderá ser considerada concluída quando:

- Todos os casos de teste planejados para o ciclo forem executados ou possuírem justificativa para bloqueio.
- Os resultados obtidos estiverem documentados.
- Os bugs identificados estiverem registrados e classificados.
- As evidências estiverem organizadas e acessíveis.
- Os problemas críticos identificados estiverem destacados no relatório final.
- As possíveis correções forem reavaliadas quando disponibilizadas.
- O relatório final apresentar o resumo dos testes e as principais recomendações.

**Observação:** a conclusão do trabalho acadêmico não significa necessariamente que todos os defeitos foram corrigidos, mas que foram identificados, analisados e documentados dentro do escopo definido.

---


---

## 🐞 7. Gestão de Defeitos

Durante os testes, os comportamentos que não atenderem aos critérios esperados serão documentados por meio de relatórios de bugs.

Cada defeito deverá conter:

1. **ID e título:** identificação e resumo da falha.
2. **Descrição:** detalhamento do problema encontrado.
3. **Severidade:** impacto da falha sobre o funcionamento do sistema.
4. **Prioridade:** urgência recomendada para correção.
5. **Status:** situação atual do defeito.
6. **Passos para reproduzir:** sequência de ações realizadas.
7. **Comportamento esperado:** resultado que deveria ocorrer.
8. **Comportamento obtido:** resposta apresentada pelo sistema.
9. **Ambiente de teste:** navegador, sistema operacional e módulo.
10. **Evidências:** capturas de tela e gravações.
11. **Caso de teste relacionado:** referência ao cenário no qual a falha foi identificada.

### Classificação de severidade

| Severidade | Descrição |
|---|---|
| **Crítica** | Compromete gravemente a segurança, a integridade dos dados ou a disponibilidade do sistema. |
| **Alta** | Impede a execução de uma funcionalidade importante ou compromete significativamente sua utilização. |
| **Média** | Afeta parcialmente a funcionalidade ou prejudica a experiência do usuário sem necessariamente impedir a operação. |
| **Baixa** | Apresenta impacto limitado, normalmente relacionado a pequenos ajustes visuais ou comportamentais. |

Os defeitos serão acompanhados por meio da documentação no GitHub, mantendo o vínculo com os casos de teste e as respectivas evidências.

---

## ⚠️ 8. Riscos Identificados

| Risco | Impacto | Estratégia de mitigação |
|---|---|---|
| Indisponibilidade temporária do sistema | Alto | Registrar a ocorrência e reagendar a execução. |
| Erros internos durante a navegação | Alto | Documentar a falha, o tempo de sessão e as ações realizadas. |
| Expiração inesperada da sessão | Médio | Verificar o comportamento após nova autenticação e registrar evidências. |
| Alterações nos dados por outros usuários | Médio | Utilizar registros de teste identificáveis e conferir o estado dos dados antes da execução. |
| Falhas de validação em formulários | Médio | Executar cenários positivos e negativos e registrar os resultados. |
| Inconsistências em indicadores e relatórios | Alto | Comparar informações da interface com registros disponíveis e consultas autorizadas ao banco. |
| Exclusão acidental de informações | Alto | Evitar operações destrutivas em dados reais e utilizar registros controlados. |
| Limitações de permissões do usuário | Médio | Documentar funcionalidades indisponíveis ou casos bloqueados. |
| Falhas na gravação de evidências | Médio | Conferir imagens e vídeos após cada execução. |
| Exposição de dados pessoais nas evidências | Alto | Ocultar informações sensíveis antes da publicação no GitHub. |

---

## 📁 9. Entregáveis

Ao final do processo, o projeto deverá apresentar os seguintes materiais:

| Entregável | Descrição |
|---|---|
| 📄 **Plano de Testes** | Documento com estratégia, escopo, objetivos, critérios e riscos. |
| 📦 **Requisitos Funcionais** | Levantamento das funcionalidades avaliadas no SIFIT. |
| 🧪 **Casos de Teste** | Cenários estruturados com pré-condições, passos e critérios de aceitação. |
| 📸 **Evidências de Execução** | Prints e vídeos que demonstram os comportamentos observados. |
| 🐞 **Relatórios de Bugs** | Registros detalhados das falhas encontradas. |
| 💡 **Recomendações de Melhoria** | Sugestões relacionadas à funcionalidade, usabilidade e tratamento de erros. |
| 📊 **Relatório Final de QA** | Consolidado dos testes executados, resultados e principais conclusões. |

---

## 👩‍💻 10. Considerações Finais

O plano de testes do SIFIT foi elaborado com o objetivo de orientar a execução das atividades de Quality Assurance, proporcionando organização, rastreabilidade e padronização na documentação.

A avaliação das funcionalidades será realizada considerando tanto o comportamento técnico do sistema quanto a experiência do usuário durante a utilização.

Os resultados obtidos permitirão identificar problemas, registrar evidências e apresentar recomendações para melhoria da qualidade do software.

Por meio desse processo, o projeto também contribui para o desenvolvimento de competências práticas em análise de requisitos, planejamento de testes, execução manual, identificação de defeitos e documentação técnica.

**Status do Plano de Testes:** Em andamento — Outubro de 2026.
