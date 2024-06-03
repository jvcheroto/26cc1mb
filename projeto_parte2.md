
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

- **Cenário de Teste 02: Teste para identificar de Produtos que estão Indisponíveis**
  - CT01: [Dado de Entrada: Produto marcado como indisponível no sistema. Resultado Esperado: Exibição de uma mensagem clara indicando que o produto está indisponível para compra.]
  - CT02: [Dado de Entrada: Busca por um produto que está indisponível. Resultado Esperado: Produto deve aparecer na busca com uma indicação de indisponibilidade.]

# 2 - Requisitos Não Funcionais (RNF):

## RNF01: Teste de desempenho de Carregamento de Páginas
- **Cenário de Teste 01: Teste de desempenho de carregamento do catálogo de produtos**
  - CT 01: [Dado de Entrada: Acesso ao catálogo de produtos. Resultado Esperado: A página deve carregar em no máximo 2 segundos.]

- **Cenário de Teste 02: Verificação da integridade e segurança dos dados dos produtos**
  - CT 01: [Dado de Entrada: Tentativa de alteração não autorizada dos dados de um produto. Resultado Esperado: O sistema deve prevenir alterações não autorizadas e garantir a segurança dos dados.]

- **Cenário de Teste 03: Teste para navegadores distintos**
  - CT 01: [Fazer o mesmo login em navegadores distintos], [Mantém a mesma conta logada nos diferentes navegadores]
  - CT 02: [Abrir outro cliente em um navegador diferente], [A sessão anterior no primeiro navegador não é atrapalhada]
  - CT 03: [Abrir o mesmo cliente ou outro cliente em uma guia anônima], [Não interrompe nem atrapalha a navegação no primeiro navagador]


## RNF02: Segurança
- **Cenário de teste 01: Teste de login seguro**
  - CT 01: [Tentar fazer login com credenciais válidas, conexão SSL ativada]
  - CT 02: [Tentar fazer login com credenciais inválidas, conexão SSL ativada]
  - CT 03: [Tentar fazer login sem HTTPS, conexão não permitida]
  
- **Cenário de teste 02: Teste de checkout seguro**
  - CT 01: [Adicionar itens ao carrinho e proceder para o checkout, conexão SSL ativada]
  - CT 02: [Tentar acessar informações de checkout sem HTTPS, conexão não permitida]
  - CT 03: [Realizar transação de pagamento, conexão SSL ativada]

## RNF03: Confiabilidade
- **Cenário de teste 01: Teste de estabilidade do servidor**
  - CT 01: [Simular 100 usuários acessando simultaneamente a página inicial do site durante 1 hora, garantindo que o tempo de resposta médio seja inferior a 3 segundos.]
  - CT 02: [Aumentar gradualmente a carga de 500 para 1000 usuários em um período de 2 horas e verificar se não há aumento significativo no tempo de resposta ou erros de servidor.]
  - CT 03: [Simular um pico de tráfego repentino dobrando o número de usuários ativos em 5 minutos e monitorar como o servidor responde, garantindo que o sistema não fique sobrecarregado e continue operacional.]
  
- **Cenário de teste 02: Teste de backup e recuperação**
  - CT 01: [Realizar um backup completo dos dados do site e restaurá-lo em um ambiente de teste, verificando se todos os dados são recuperados corretamente e nenhum dado é perdido durante o processo.]
  - CT 02: [Simular uma falha no servidor principal e iniciar o processo de recuperação a partir do último backup, garantindo que o tempo de recuperação seja inferior a 1 hora e todos os serviços sejam restaurados.]
  - CT 03: [Testar a validade dos backups realizados verificando se os arquivos de backup estão completos, não corrompidos e podem ser restaurados conforme necessário.]

- **Cenário de teste 03: Teste de disponibilidade**
  - CT 01: [Monitorar o tempo de atividade do site 24/7, registrando qualquer interrupção de serviço e garantindo que o tempo de inatividade total seja inferior a 1 hora por mês.]
  - CT 02: [Testar o failover para servidores de backup em caso de falha do servidor principal, garantindo uma transição suave e que os usuários não percebam a mudança de servidor.]
  - CT 03: [Realizar testes de recuperação de desastres simulando situações de emergência, como ataques DDoS, e garantir que o site permaneça acessível e funcional durante e após o evento.]

# 3 - Componentes:

| Aluno                        | Professora                | Turma | Disciplina                     |
| ---------------------------- | ------------------------- | ----- | ------------------------------ |
| João Victor Piumbini Cheroto | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
| Rodrigo da Cunha             | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
| Luiz Fernando Sacht          | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
