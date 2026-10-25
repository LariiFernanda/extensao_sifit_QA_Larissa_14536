
## Cenário 04: Gestão de Clientes.

### Caso de Teste 01: Adicionar novo Cliente com dados válidos.

| ID       | Descrição                                                          |
| :------- | :----------------------------------------------------------------- |
| C03-CT01 | O sistema deve permitir o cadastro de um Cliente com dados válidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo PIM.       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** clica em \"Novo Cliente\"                                  |
| **E** preenche \"Larissa\" no campo Nome  |
| **QUANDO** clicar em \"Salvar\"                                    |
| **ENTÃO** o Cliente deve ser cadastrado e exibido na lista  |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O Cliente deve aparecer corretamente listado no módulo. |

**Resultado obtido:** CLIENTE CADASTRADO COM SUCESSO, SEM SER PREENCHIDO TODOS OS CAMPOS NECESSÁRIOS COMO DOCUMENTO E ENDEREÇO
ALÉM DE O CAMPO (RG) PERMITIR VÁRIOS CARACTERES, INVIABILIZANDO O NUMERO CORRETO  DE 7 A 9 DIGITOS VÁLIDOS PARA O DOCUMENTO.
Status: REPROVADO .

|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução: 
https://jam.dev/c/e80c3431-f139-4866-b7b8-ab13a9718ef6

---

### Caso de Teste 02: Tentar adicionar Cliente sem preencher campos obrigatórios.

| ID       | Descrição                                                                  |
| :------- | :------------------------------------------------------------------------- |
| C03-CT02 | O sistema deve exibir erros ao tentar salvar um Cliente sem preencher os campos obrigatórios. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa a tela de \"Novo Cliente\"          |
| **E** deixa os campos obrigatórios em branco                     |
| **QUANDO** clicar em \"Salvar\"                                    |
| **ENTÃO** mensagens de erro devem ser exibidas nos campos obrigatórios |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem exibir mensagens de validação.     |

**Resultado obtido:** O Sistema permite cadastrar um novo Cliente preenchendo apenas o nome, sexo, status, data de nascimento.
Sem que os demais campos importantes estivessem preenchidos.
OUTRA OBSERVAÇÃO IMPORTANTE É QUE O CAMPO DO (RG) ACEITA VÁRIOS CARACTERES, ACIMA DA QUANTIDADE PERMITIDA QUE É DE 7 a 9 DÍGITOS (além do dígito verificador).

Status: REPROVADO.

|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução: 
https://jam.dev/c/e80c3431-f139-4866-b7b8-ab13a9718ef6
---

### Caso de Teste 03: Pesquisar Cliente já cadastrado.

| ID       | Descrição                                                  |
| :------- | :--------------------------------------------------------- |
| C03-CT03 | O sistema deve retornar corretamente o Cliente pesquisado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O Cliente deve já estar cadastrado no sistema.            |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** digita \"Larissa\" no campo de busca                      |
| **QUANDO** clicar no botão \"Buscar\"                            |
| **ENTÃO** o sistema deve exibir \"Larissa\" na lista de resultados |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O Cliente correspondente deve ser listado corretamente.     |

**Resultado obtido:** Cliente consta na lista, e  se buscado também é encontrado, porém notei que a visualização
das informacões do cadastro não aparecem no perfim do cliente, tem que clicar em EDITAR, para visualizar os dados.

Status: Aprovado.

|                **Evidência(s)**               |
| :-------------------------------------------: |
Vídeo da execução:
https://jam.dev/c/e80c3431-f139-4866-b7b8-ab13a9718ef6
