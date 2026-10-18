# ✅ Relatório de Execução de Testes — SIFIT

## 📌 1. Identificação

| Informação | Descrição |
|---|---|
| **Sistema** | SIFIT — Gestão de Academias |
| **Responsável** | Larissa — QA |
| **Período** | Outubro de 2026 |
| **Ambiente** | [SIFIT Web](https://sifit.centrion.com.br/) |
| **Tipo de Teste** | Manual, Funcional e Exploratório |
| **Status** | Em andamento |

---

## 📊 2. Resumo da Execução

Os testes têm como objetivo verificar o funcionamento das principais funcionalidades do SIFIT, identificar falhas e avaliar a experiência do usuário.

| Indicador | Resultado |
|---|---|
| Casos planejados | Em levantamento |
| Casos executados | Em consolidação |
| Casos aprovados | Em consolidação |
| Casos reprovados | Em consolidação |
| Bugs identificados | 3 ocorrências documentadas ou em investigação |

---

## 🔍 3. Cobertura dos Testes

| Módulo | Situação |
|---|---|
| Autenticação | Testado |
| Página Inicial e Dashboard | Testado |
| Check-in e Presenças | Em investigação |
| Clientes e Matrículas | Pendente de consolidação |
| Avaliações e Treinamentos | Pendente de consolidação |
| Gestão Financeira | Pendente de consolidação |
| Turmas e SifitBox | Pendente de consolidação |
| Cadastros Administrativos | Pendente de consolidação |
| Inteligência e Automação | Pendente de consolidação |

---

## 🐞 4. Bugs Identificados

| ID | Descrição | Severidade sugerida |
|---|---|---|
| BUG-001 | Mensagem inadequada ao tentar login com campos vazios. | Média |
| BUG-C02-001 | Baixo contraste nos textos e gráficos do Dashboard. | Média |
| BUG-002 | Erro interno do servidor durante a navegação após mais de uma hora de sessão. | Alta (provisória) |

**Observação:** o erro interno ainda está em investigação. Não foi confirmado que o tempo de sessão seja sua causa.

---

## 📈 5. Resultados Obtidos

Durante os testes, foi possível confirmar o funcionamento da autenticação com credenciais válidas, o bloqueio de acessos incorretos e o carregamento das informações gerenciais.

Entretanto, foram identificadas inconsistências relacionadas à validação de campos obrigatórios, à legibilidade dos gráficos e ao tratamento de erros internos.

Esses problemas foram registrados para análise e recomendações de melhoria.

---

## 📁 6. Evidências

As execuções são documentadas por meio de capturas de tela, gravações e relatórios de bugs, organizados no GitHub.

- 📸 Prints dos testes realizados.
- 🎥 [Evidência de erro interno — Jam.dev](https://jam.dev/c/f57b5c39-dcf1-49ec-bdda-a0b42f85d11a)
- 🧪 Casos de teste em BDD (DADO, QUANDO e ENTÃO).
- 🐞 Relatórios individuais de defeitos.

---

## 🔎 7. Análise de Causa Raiz (RCA)

A análise de causa raiz busca identificar os fatores responsáveis pelas falhas encontradas.

No SIFIT, as principais hipóteses de investigação envolvem validações de formulários, configurações visuais dos gráficos e possíveis problemas na comunicação com o servidor ou gerenciamento de sessões.

A confirmação dessas causas depende de investigação técnica e, quando disponível, da análise dos logs do sistema.

---

## ✅ 8. Conclusão

Os testes manuais realizados até o momento demonstraram que o SIFIT possui funcionalidades operacionais, mas também apresenta inconsistências que podem comprometer a experiência do usuário.

Os problemas identificados foram documentados com evidências, permitindo orientar futuras correções e melhorias.

**O processo de QA permanece em andamento**, com novos testes previstos para os demais módulos do sistema.
