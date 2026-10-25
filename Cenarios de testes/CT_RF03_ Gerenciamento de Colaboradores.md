## Cenário 03: Gestão de funcionários via módulo PIM.

### Caso de Teste 01: Adicionar novo funcionário com dados válidos.

| ID       | Descrição                                                          |
| :------- | :----------------------------------------------------------------- |
| C03-CT01 | O sistema deve permitir o cadastro de um funcionário com dados válidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo PIM.       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** clica em \"Novo Colaborador\"                                  |
| **E** preenche \"Larissa\" no campo Nome  |
| **QUANDO** clicar em \"Salvar\"                                    |
| **ENTÃO** o funcionário deve ser cadastrado e exibido na lista do PIM |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O funcionário deve aparecer corretamente listado no módulo PIM. |

**Resultado obtido:**
Cadastro realizado com sucesso, porém não apresenta campos obrigatórios.
E o status deve ser selecionado ATIVO/INATIVO.

Status: Aprovado.

|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução: 
https://jam.dev/c/15fbb3d6-0290-48f5-9463-d5d177273308

---

### Caso de Teste 02: Tentar adicionar funcionário sem preencher campos obrigatórios.

| ID       | Descrição                                                                  |
| :------- | :------------------------------------------------------------------------- |
| C03-CT02 | O sistema deve exibir erros ao tentar salvar um funcionário sem preencher os campos obrigatórios. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa a tela de \"Add Colaboradores\"          |
| **E** deixa os campos obrigatórios em branco                     |
| **QUANDO** clicar em \"Salvar\"                                    |
| **ENTÃO** mensagens de erro devem ser exibidas nos campos obrigatórios |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem exibir mensagens de validação.     |

**Resultado obtido:** O Sistema permite cadastrar um novo colaborador preenchendo apenas o nome, sexo, status, data de nascimento.
Sem que os demais campos importantes estivessem preenchidos.
OUTRA OBSERVAÇÃO IMPORTANTE É QUE O CAMPO DO (RG) ACEITA VÁRIOS CARACTERES, ACIMA DA QUANTIDADE PERMITIDA QUE É DE 7 a 9 DÍGITOS (além do dígito verificador).

Status: REPROVADO.

|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução: 
https://jam.dev/c/3c9d7444-af97-4999-b85b-ac86bcdc8288
---

### Caso de Teste 03: Pesquisar funcionário já cadastrado.

| ID       | Descrição                                                  |
| :------- | :--------------------------------------------------------- |
| C03-CT03 | O sistema deve retornar corretamente o funcionário pesquisado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O funcionário deve já estar cadastrado no sistema.            |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** digita \"Larissa\" no campo de busca                      |
| **QUANDO** clicar no botão \"Buscar\"                            |
| **ENTÃO** o sistema deve exibir \"Larissa\" na lista de resultados |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O funcionário correspondente deve ser listado corretamente.     |

Status: Aprovado.

|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução:
https://jam.dev/c/679b3190-769f-4386-862a-667b7b4e418d
