# Cenário 07: Gerenciamento de Relatórios

---

## Caso de Teste CT01: Gerar relatório de avaliações físicas

| ID | Descrição |
|---|---|
| **RF07-CT01** | Verificar se o sistema SIFIT permite gerar relatórios contendo o histórico de avaliações físicas dos clientes. |

| Pré-condições |
|---|
| O usuário deve estar autenticado e possuir permissão para acessar relatórios. Devem existir avaliações físicas cadastradas no sistema. |

| Passos |
|---|
| DADO que estamos na página de Relatórios do SIFIT |
| E selecionamos a opção "Avaliações" no campo "Tipo de Relatório" |
| E informamos os filtros disponíveis |
| QUANDO solicitarmos a geração do relatório |
| ENTÃO o sistema deverá gerar o relatório de avaliações físicas |

| Critérios de aceitação |
|---|
| O relatório deve apresentar os registros de avaliações correspondentes aos filtros selecionados, sem omitir registros válidos ou apresentar dados de avaliações não relacionadas à consulta. |

| Resultado obtido |
|---|
|  Ao filtrar a busca do relatório por Tipo e data, ao clicar em gerar relatório o PDF, baixou automático porém não abriu. Deu ERRO. |

| Status |
|---|
| ❌ Reprovado |

| Evidência(s) |
|---|
Vídeo:
|https://jam.dev/c/3a79f231-36e8-4cf7-a95e-3fb1c9f5b2ff|

---

## Caso de Teste CT02: Gerar relatório de clientes

| ID | Descrição |
|---|---|
| **RF07-CT02** | Verificar se o sistema permite gerar um relatório contendo os clientes cadastrados e suas respectivas situações. |

| Pré-condições |
|---|
| O usuário deve possuir acesso ao módulo de Relatórios e devem existir clientes cadastrados. |

| Passos |
|---|
| DADO que estamos na página de Relatórios |
| E selecionamos a opção "Clientes" |
| E configuramos os filtros disponíveis |
| QUANDO solicitarmos a geração do relatório |
| ENTÃO o sistema deverá apresentar os dados dos clientes correspondentes à consulta |

| Critérios de aceitação |
|---|
| O relatório deve apresentar corretamente os clientes e suas situações cadastrais, respeitando os filtros informados e as permissões do usuário. |

| Resultado obtido |
|---|
| Ao filtrar a busca do relatório por Tipo e data, ao clicar em gerar relatório o PDF, baixou automático porém não abriu. Deu ERRO. |

| Status |
|---|
| ❌ Reprovado |

| Evidência(s) |
|---|
Vídeo:
| https://jam.dev/c/3a79f231-36e8-4cf7-a95e-3fb1c9f5b2ff |

---

## Caso de Teste CT03: Gerar relatório de colaboradores

| ID | Descrição |
|---|---|
| **RF07-CT03** | Verificar se o sistema permite gerar relatórios com informações dos colaboradores cadastrados. |

| Pré-condições |
|---|
| O usuário deve possuir permissão para consultar informações de colaboradores e devem existir colaboradores cadastrados. |

| Passos |
|---|
| DADO que estamos na página de Relatórios |
| E selecionamos o tipo "Colaboradores" |
| E definimos os filtros disponíveis |
| QUANDO solicitarmos a geração do relatório |
| ENTÃO o sistema deverá apresentar os colaboradores correspondentes à consulta |

| Critérios de aceitação |
|---|
| O relatório deve apresentar os colaboradores corretos, com informações coerentes com seus registros cadastrais e sem expor dados restritos a usuários não autorizados. |

| Resultado obtido |
|---|
| Ao filtrar a busca do relatório por Tipo e data, ao clicar em gerar relatório o PDF, baixou automático porém não abriu. Deu ERRO. |

| Status |
|---|
| ❌ Reprovado |

| Evidência(s) |
|---|
Vídeo:
| https://jam.dev/c/3a79f231-36e8-4cf7-a95e-3fb1c9f5b2ff |
