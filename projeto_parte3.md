# Relatório de Testes - Site Casa & Vídeo

### Caso de Teste 01

- **Nome do requisito:** Cadastro de usuário
- **Cenário de teste:** Cadastro de conta usando dados válidos
- **Resultado obtido:** O site realizou o cadastro com sucesso, porém não foi mostrada uma mensagem de cadastro realizado com sucesso.
- **Status:** Passou

### Caso de Teste 02

- **Nome do requisito:** Cadastro de usuário
- **Cenário de teste:** Cadastro de conta usando um e-mail falso
- **Resultado obtido:** Usando o email falso: exemplo@mail.com, o site entende como um email existente.
- **Status:** Falhou

### Caso de Teste 03

- **Nome do requisito:** Cadastro de usuário
- **Cenário de teste:** Cadastro com senha que não correspondem
- **Resultado obtido:** Usando uma senha diferente da outra o site passa a seguinte mensagem: confirmação de senha incorreta. 
- **Status:** Passou
