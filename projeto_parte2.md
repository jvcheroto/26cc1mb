
# 1 - Requisitos Funcionais (RF):

## RF001: Cadastro de usuário
- **Cenário de Teste 01: Cadastro com dados válidos**
  - CT01: [Nome: "João Silva", Email: "joao.silva@example.com", Senha: "Senha123!", Confirmação de Senha: "Senha123!", Resultado Esperado: Cadastro realizado com sucesso, e-mail de confirmação enviado]
  - CT02: [Nome: "Maria Santos", Email: "maria.santos@example.com", Senha: "Senha@456", Confirmação de Senha: "Senha@456", Resultado Esperado: Cadastro realizado com sucesso, e-mail de confirmação enviado]


- **Cenário de Teste 02: Cadastro com e-mail inválido**
  - CT01: [Nome: "Ana Pereira", Email: "ana.pereiraexample.com", Senha: "Senha789!", Confirmação de Senha: "Senha789!", Resultado Esperado: Mensagem de erro "Formato de e-mail inválido"]
  - CT02: [Nome: "Carlos Lima", Email: "carlos.lima@.com", Senha: "Senha@101", Confirmação de Senha: "Senha@101", Resultado Esperado: Mensagem de erro "Formato de e-mail inválido"]


- **Cenário de Teste 03: Cadastro com senhas não correspondentes**
  - CT01: [Nome: "Pedro Sousa", Email: "pedro.sousa@example.com", Senha: "Senha202", Confirmação de Senha: "Senha303", Resultado Esperado: Mensagem de erro "As senhas não correspondem"]
  - CT02: [Nome: "Rita Nunes", Email: "rita.nunes@example.com", Senha: "Senha@404", Confirmação de Senha: "Senha@505", Resultado Esperado: Mensagem de erro "As senhas não correspondem"]
 
- **Cenário de Teste 04: Cadastro com senha fraca**
  - CT01: [Nome: "Laura Dias", Email: "laura.dias@example.com", Senha: "1234", Confirmação de Senha: "1234", Resultado Esperado: Mensagem de erro "A senha deve ter pelo menos 8 caracteres, incluindo letras maiusculas, minúsculas e números"]
  - CT02: [Nome: "Fabio Melo", Email: "fabio.melo@example.com", Senha: "abcdef", Confirmação de Senha: "abcdef", Resultado Esperado: Mensagem de erro "A senha deve ter pelo menos 8 caracteres, incluindo letras maiusculas, minúsculas e números"]




## RF002: Carrinho de Compras
- **Cenário de Teste 01: Adicionar produtos ao carrinho**
  - CT01: [Produto: "TV 40 Polegadas", Quantidade: 1, Resultado Esperado: Produto adicionado ao carrinho com sucesso]
  - CT02: [Produto: "Notebook 15 Polegadas", Quantidade: 1, Resultado Esperado: Produto adicionado ao carrinho com sucesso]


- **Cenário de Teste 02: Editar a quantidade de produtos no carrinho**
  - CT01 [Produto: "TV 40 Polegadas", Quantidade Inicial: 1, Quantidade Editada: 2, Resultado Esperado: Quantidade de produtos atualizada no carrinho]
  - CT02: [Produto: "Notebook 15 Polegadas", Quantidade Inicial: 1, Quantidade Editada: 3, Resultado Esperado: Quantidade de produtos atualizada no carrinho]

- **Cenário de Teste 03: Remover itens do carrinho**
  - CT01: [Produto: "TV 40 Polegadas", Ação: Remover, Resultado Esperado: Produto removido do carrinho]
  - CT02: [Produto: "Notebook 15 Polegadas", Ação: Remover, Resultado Esperado: Produto removido do carrinho]

- **Cenário de Teste 04: Proceder para o checkout**
  - CT01: [Itens no Carrinho: "TV 40 Polegadas" (2), "Notebook 15 Polegadas" (1), Resultado Esperado: Usuário redirecionado para a página de checkout com os itens corretos e resumo do pedido]

# 2 - Requisitos Não Funcionais (RNF):

## RNF001: Compatibilidade de Navegadores
- **Cenário de Teste 01: Acessar o portal**
  - CT 01: [Acessar o portal via Google Chrome], [Acesso feito com sucesso]
  - CT 02: [Acessar o portal via Microsoft Edge], [Acesso feito com sucesso]
  - CT 03: [Acessar o portal via Mozilla Firefox], [Acesso feito com sucesso]
  - CT 04: [Acessar o portal via Safari], [Acesso feito com sucesso]
  - CT 05: [Acessar o portal via Opera GX], [Acesso feito com sucesso]
  - **OBS:** Não foi realizado em todos os navegadores existentes, mas os citados acima são os mais comuns e funcionaram.

- **Cenário de Teste 02: Uso de diferentes guias**
  - CT 01: [Abrir uma tela interna em uma nova guia], [Mantém o login atual]
  - CT 02: [Duplicar a guia], [Mantém a mesma tela e progresso de um determinado processo na guia que foi duplicada]
  - CT 03: [Abrir uma tela interna em uma guia anônima], [A opção fica desabilitada]
  - CT 04: [Fazer login em outro cliente em uma nova guia], [A sessão anterior é desconectada, mantêm-se a nova]
  - CT 05: [Abrir o mesmo cliente ou outro cliente em uma guia anônima], [Não interrompe nem atrapalha a navegação que não é anônima]

- **Cenário de Teste 03: Navegadores distintos**
  - CT 01: [Fazer o mesmo login em navegadores distintos], [Mantém a mesma conta logada nos diferentes navegadores]
  - CT 02: [Abrir outro cliente em um navegador diferente], [A sessão anterior no primeiro navegador não é atrapalhada]
  - CT 03: [Abrir o mesmo cliente ou outro cliente em uma guia anônima], [Não interrompe nem atrapalha a navegação no primeiro navagador]


## RNF002: Integração
- **Cenário de Teste 01: Integração via SOAP/API Rest (SoapUI/Postman) - externo à plataforma**
  - CT 01: [Enviar usuário e senha de integração corretos], [Código 200 (OK)]
  - CT 02: [Enviar usuário correto e senha em branco], [Erro: Código 401 (Unauthorized)]
  - CT 03: [Enviar usuário em branco e senha correta], [Erro: Código 401 (Unauthorized)]
  - CT 04: [Não preencher as credenciais], [Erro: Código 401 (Unauthorized)]
  - CT 05: [Não enviar a tag de integração], [Nos programas aparece código 200 (OK), porém a integração não é feita na plataforma]
    - **Resposta da plataforma:** "Não existe ID relacionado à TAG:"
  - CT 06: [Enviar um valor não válido na tag de integração], [Nos programas aparece código 200 (OK), porém a integração não é feita na plataforma]
    - **Resposta da plataforma:** "Não existe ID relacionado à TAG: TESTE"
  - CT 07: [Não enviar uma tag obrigatória (Ex.: REQUISICAOCLIENTE)], [Nos programas aparece código 200 (OK), porém a integração não é feita na plataforma]
    - **Resposta da plataforma:** "Erro na entrada de requisição 0: Numero da requisicao cliente não informado."
  - CT 08: [Enviar uma tag incorreta], [Erro: Código 400 (Bad Request)]
  - CT 09: [Enviar uma tag que não existe], [A integração é feita com sucesso (Código 200), logo a plataforma apenas ignorou a tag inexistente]

- **Cenário de Teste 02: Integração via Planilhas do Excel (Cargas) - interno à plataforma**
  - CT 01: [Enviar todas as colunas e abas com os devidos nomes e valores válidos e aceitos], [Status Processado]
    - **OBS:** A plataforma utiliza a terminologia *"Processado"* para indicar sucesso no envio da carga.
  - CT 02: [Enviar com dados inválidos], [Erro: Status Erro]
  - CT 03: [Enviar sem abas obrigatórias], [Erro: Status Erro]
  - CT 04: [Enviar sem colunas obrigatórias], [Erro: Status Erro]
  - CT 05: [Enviar tipo de dado incorretos em determinadas colunas], [Erro: Status Erro]
  - CT 06: [Enviar coluna inexistente], [Erro: Status Erro]


# 3 - Componentes:

| Aluno                        | Professora                | Turma | Disciplina                     |
| ---------------------------- | ------------------------- | ----- | ------------------------------ |
| João Victor Piumbini Cheroto | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
| Rodrigo da Cunha             | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
| Luiz Fernando Sacht          | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
