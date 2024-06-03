
# 1 - Requisitos Funcionais (RF):

## RF001: Cadastro de usuário
- **Cenário de Teste 01: Cadastro de conta usando dados válidos**
  - CT01: [Nome: "João Silva", Email: "joao.silva@example.com", Senha: "Senha123!", Confirmação de Senha: "Senha123!", Resultado Esperado: Cadastro realizado com sucesso, e-mail de confirmação enviado]
  - CT02: [Nome: "Maria Santos", Email: "maria.santos@example.com", Senha: "Senha@456", Confirmação de Senha: "Senha@456", Resultado Esperado: Cadastro realizado com sucesso, e-mail de confirmação enviado]


- **Cenário de Teste 02: Cadastro de conta usando um e-mail falso**
  - CT01: [Nome: "Ana Pereira", Email: "ana.pereiraexample.com", Senha: "Senha789!", Confirmação de Senha: "Senha789!", Resultado Esperado: Mensagem de erro "Entre com um e-mail válido"]
  - CT02: [Nome: "Carlos Lima", Email: "carlos.lima@.com", Senha: "Senha@101", Confirmação de Senha: "Senha@101", Resultado Esperado: Mensagem de erro "Entre com um e-mail válido"]


- **Cenário de Teste 03: Cadastro com senhas que não correspondentes**
  - CT01: [Nome: "Pedro Sousa", Email: "pedro.sousa@example.com", Senha: "Senha202", Confirmação de Senha: "Senha303", Resultado Esperado: Mensagem de erro "As senhas não correspondem"]
  - CT02: [Nome: "Rita Nunes", Email: "rita.nunes@example.com", Senha: "Senha@404", Confirmação de Senha: "Senha@505", Resultado Esperado: Mensagem de erro "As senhas não correspondem"]
 
- **Cenário de Teste 04: Teste de cadastro com senha "fraca"**
  - CT01: [Nome: "Laura Dias", Email: "laura.dias@example.com", Senha: "1234", Confirmação de Senha: "1234", Resultado Esperado: Mensagem de erro "A senha deve ter pelo menos 8 caracteres, incluindo letras maiusculas, minúsculas e números"]
  - CT02: [Nome: "Fabio Melo", Email: "fabio.melo@example.com", Senha: "abcdef", Confirmação de Senha: "abcdef", Resultado Esperado: Mensagem de erro "A senha deve ter pelo menos 8 caracteres, incluindo letras maiusculas, minúsculas e números"]




## RF002: Carrinho de Compras
- **Cenário de Teste 01: Teste ao adicionar produtos ao carrinho**
  - CT01: [Produto: "TV 40 Polegadas", Quantidade: 1, Resultado Esperado: Produto adicionado ao carrinho com sucesso]
  - CT02: [Produto: "Notebook 15 Polegadas", Quantidade: 1, Resultado Esperado: Produto adicionado ao carrinho com sucesso]


- **Cenário de Teste 02: Editar a quantidade de produtos no carrinho**
  - CT01 [Produto: "TV 40 Polegadas", Quantidade Inicial: 1, Quantidade Editada: 2, Resultado Esperado: Quantidade de produtos atualizada no carrinho]
  - CT02: [Produto: "Notebook 15 Polegadas", Quantidade Inicial: 1, Quantidade Editada: 3, Resultado Esperado: Quantidade de produtos atualizada no carrinho]

- **Cenário de Teste 03: Teste de remover itens do carrinho**
  - CT01: [Produto: "TV 40 Polegadas", Ação: Remover, Resultado Esperado: Produto removido do carrinho]
  - CT02: [Produto: "Notebook 15 Polegadas", Ação: Remover, Resultado Esperado: Produto removido do carrinho]

- **Cenário de Teste 04: Teste de continuar para o checkout**
  - CT01: [Itens no Carrinho: "TV 40 Polegadas" (2), "Notebook 15 Polegadas" (1), Resultado Esperado: Usuário redirecionado para a página de checkout com os itens corretos e resumo do pedido]

## RF003:  Exibição Correta do Catálogo de Produtos
- **Cenário de Teste 01: Verificação da Exibição Correta do Catálogo de Produtos**
  - CT01: [Dado de Entrada: Acesso à categoria "Televisões e Smart TVs". Resultado Esperado: Exibição de produtos apenas da categoria "Televisões e Smart TVs".]
  - CT02: [Dado de Entrada: Navegação dentro da categoria "Televisões e Smart TVs". Resultado Esperado: Não deve haver produtos de outras categorias, como aspiradores de pó.]

- **Cenário de Teste 02: Teste para identificar os Produtos que estão indisponíveis**
  - CT01: [Dado de Entrada: Produto marcado como indisponível no sistema. Resultado Esperado: Exibição de uma mensagem clara indicando que o produto está indisponível para compra.]
  - CT02: [Dado de Entrada: Busca por um produto que está indisponível. Resultado Esperado: Produto deve aparecer na busca com uma indicação de indisponibilidade.]

## RF004: Exibição Correta dos Produtos em Promoção no Catálogo

- **Cenário de Teste 01: Verificação da Exibição dos Produtos em Promoção**
  - CT01: [Dado de Entrada: Acesso à seção de produtos em promoção. Resultado Esperado: Exibição apenas dos produtos que estão em promoção.]
  - CT02: [Dado de Entrada: Verificação da quantidade de produtos exibidos em promoção. Resultado Esperado: A quantidade de produtos exibidos corresponde à quantidade real de produtos em promoção no sistema.]

- **Cenário de Teste 02: Verificação dos Descontos Aplicados no Carrinho**
  - CT03: [Dado de Entrada: Adição de produtos em promoção ao carrinho. Resultado Esperado: Os descontos correspondentes devem ser aplicados corretamente ao total do carrinho.]
  - CT04: [Dado de Entrada: Verificação dos detalhes do carrinho após a aplicação dos descontos. Resultado Esperado: O valor total do carrinho reflete os descontos aplicados nos produtos em promoção.]


# 2 - Componentes:

| Aluno                        | Professora                | Turma | Disciplina                     |
| ---------------------------- | ------------------------- | ----- | ------------------------------ |
| João Victor Piumbini Cheroto | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
| Rodrigo da Cunha             | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
| Luiz Fernando Sacht          | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
