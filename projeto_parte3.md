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

### Caso de Teste 04

- **Nome do requisito:** Cadastro de usuário
- **Cenário de teste:** Cadastro com senha "fraca"
- **Resultado obtido:** O site possui um sistema de validação de senha e por isso não autoriza a criação de contas quando as senhas não preenchem os requisitos de senha "forte".
- **Status:** Passou

### Caso de Teste 05

- **Nome do requisito:** Carrinho de compras 
- **Cenário de teste:** Testar a funcionalidade do carrinho
- **Resultado obtido:** Ao adicionar produtos no carrinho a funcionalidade funciona corretamente. Só não exibe a mensagem "produto adicionado com sucesso!"
- **Status:** Passou

### Caso de Teste 06

- **Nome do requisito:** Carrinho de compras 
- **Cenário de teste:** Testar se é possivel editar a quantidade de produtos no carrinho
- **Resultado obtido:** Ao adicionar mais quantidades do mesmo produto ocorre um bug no carrinho. Ele automaticamente adiciona o mesmo produto novamente no carrinho, ou seja, existem 2 PS5 no carrinho sendo um deles com quantidade 5 e outro com 1 somente.
- **Status:** Falhou

### Caso de Teste 07

- **Nome do requisito:** Carrinho de compras 
- **Cenário de teste:** Testar se é possivel retirar produtos do carrinho
- **Resultado obtido:** A função de retirar o produto não funciona corretamente quando ocorre o bug anterior. O produto duplicado permanece no carinho e o que é retirado é 1 dos 5 outros PS5.
- **Status:** Falhou
