# Plano de Teste

**CASA & VIDEO**

## Sobre Casa & Video

O site da Casa & Video oferece uma ampla variedade de produtos para o lar, desde eletrodomésticos até itens de decoração. Criado com o objetivo de fornecer uma plataforma conveniente e acessível para compras online, a Casa & Video atende às necessidades dos consumidores que buscam qualidade, variedade e preços competitivos para equipar e decorar suas casas.

## 1 - Introdução

Este documento descreve o plano de testes para o site da Casa & Vídeo. O objetivo deste plano é garantir que todas as funcionalidades do site estejam funcionando corretamente, proporcionando uma experiência de compra satisfatória aos usuários.

Este plano de testes abordará diferentes aspectos do site, incluindo navegação, funcionalidades de pesquisa, adição de produtos ao carrinho, processo de checkout, entre outros. Serão realizados testes manuais e automatizados para garantir uma cobertura abrangente dos cenários de uso do site.

Com esse documento, identificaremos:
- Informações de projeto existentes e os componentes de software que devem ser testados.
- Listar os Requisitos a testar.
- Recomendar e descrever as estratégias de teste a serem empregadas.
- Recursos necessários e prover uma estimativa dos esforços de teste.
- Listar os elementos resultantes do projeto de testes.

## 2 - Requisitos Funcionais

Esta seção contém os requisitos funcionais identificados como objetos dos testes ao longo do desenvolvimento do projeto.

Os seguintes requisitos serão testados durante a execução deste plano:

 |Requisito  | Descrição                                          |
 |-----------|----------------------------------------------------|
 |REQ-001    | Itens de promoção                                  |
 |REQ-002    | Barra de pesquisa                                  |
 |REQ-003    | Itens por categoria                                |
 |REQ-004    | Cadastro por usuário                               |
 |REQ-005    | Carrinho de compras                                |
 
 
## 3 - Testes

Esta seção irá apresentar os testes escolhidos para cada iteração do projeto. Destacando a importância da seleção cuidadosa dos testes em cada iteração, este documento visa oferecer uma visão clara das abordagens adotadas para garantir a qualidade do software ao longo do desenvolvimento.

### 3.1 - Requisito 1: Itens de promoção

#### Exploratory Testing: 

Nosso grupo decidiu realizar o teste de um item de promoção no site da Casa & Video utilizando a técnica de Exploratory Testing. Essa abordagem de teste ad hoc nos permite explorar o sistema de forma livre, descobrindo possíveis defeitos e problemas que podem não ter sido identificados em testes formais.

#### Utilização da Técnica

Ao acessar o site da Casa & Video, navegamos pela seção de promoções e escolhemos aleatoriamente um produto em oferta. Em vez de seguir um roteiro de teste predefinido, utilizamos nossa experiência e conhecimento para interagir com o item selecionado de diferentes maneiras.

#### Teste do Item de Promoção

Ao examinarmos o produto selecionado, notamos uma discrepância nos preços dos produtos. Durante o processo de finalização da compra, ao utilizar o cupom disponibilizado e o método de pagamento pix, o produto estava sendo cobrado pelo valor de R$ 336,10. No entanto, ao acessarmos a página inicial, observamos que o mesmo produto estava sendo ofertado por R$ 289,90. Essa divergência entre os valores levanta questões sobre a integridade e precisão do sistema de precificação da plataforma, bem como sobre a experiência do usuário durante o processo de compra.

#### Critérios de Teste

#### Variedade de Promoções
- Verificamos se diferentes tipos de promoções estavam sendo exibidos corretamente no site.

#### Intuitividade de Navegação
- Testamos a facilidade de navegação entre os itens de promoção e categorias relacionadas.

#### Consistência Visual
- Avaliamos se os itens de promoção mantinham uma aparência visual consistente com o restante do site.

#### Níveis de Criticidade de Defeitos

1. **Baixa**: Defeitos que têm pouco impacto na usabilidade geral do site.
2. **Média**: Defeitos que afetam parcialmente a funcionalidade do site.
3. **Alta**: Defeitos que impedem significativamente o uso do site.

#### Resultados e Ações

Após identificarmos a discrepância de preço no item de promoção, documentamos nossas descobertas. Recomendamos uma revisão abrangente dos preços dos itens de promoção e a implementação de medidas corretivas para garantir a consistência e precisão das promoções.

#### Conclusão

O teste de Exploratory Testing nos permitiu descobrir um problema relevante que poderia ter passado despercebido em testes formais. Essa abordagem flexível e baseada na experiência é uma ferramenta valiosa para garantir a qualidade e a usabilidade do site da Casa & Video, ajudando a identificar e corrigir potenciais problemas antes que impactem negativamente os usuários.

<br/>
<table>
    <tr>
        <th>
            Objetivo
        </th>
        <th colspan="4">
            Verificar se o preço da compra é o mesmo do anunciado pelo site
        </th>
    </tr>
    <tr>
        <th>
            Técnica:
        </th>
        <th colspan="2">
            (x) manual
        </th>
        <th colspan="2">
            ( ) automática
        </th>
    </tr>
    <tr>
        <th>
            Estágio do teste
        </th>
        <th>
            Integração ( )
        </th>
        <th>
            Sistema ( )
        </th>
        <th>
            Unidade (x)
        </th>
        <th>
            Aceitação ( )
        </th>
    </tr>
    <tr>
        <th>
            Abordagem do teste
        </th>
        <th colspan="2">
            Caixa branca ( )
        </th>
        <th colspan="2">
            Caixa preta (x)
        </th>
    </tr>
    <tr>
        <th>
            Responsável(is)
        </th>
        <th colspan="4">
            João Victor Piumbini Cheroto
        </th>
    </tr>
</table>
<br/>



### 3.2 - Requisito 2: Barra de Pesquisa

#### Exploratory Testing:

Nosso grupo decidiu realizar o teste da barra de busca de itens no site da Casa & Video utilizando a técnica de Exploratory Testing. Essa abordagem de teste ad hoc nos permite explorar o sistema de forma livre, descobrindo possíveis defeitos e problemas que podem não ter sido identificados em testes formais.

#### Utilização da Técnica:

Ao acessar o site da Casa & Video, focamos em interagir com a barra de busca de itens localizada na parte superior da página. Em vez de seguir um roteiro de teste predefinido, utilizamos nossa experiência e conhecimento para explorar diferentes funcionalidades e cenários de uso da barra de busca.

#### Teste da Barra de Pesquisa:

Durante nossos testes, observamos o comportamento da barra de busca ao inserir termos e palavras-chave relacionados aos produtos disponíveis no site. Verificamos também a resposta da barra de busca ao fornecer sugestões de pesquisa e ao aplicar filtros avançados ou refinamentos de busca.

#### Critérios de Teste:

- **Presença e Acessibilidade**: Verificamos se a barra de busca estava presente em todas as páginas do site e se era facilmente acessível aos usuários.
- **Funcionalidade da Busca**: Testamos se a busca retornava resultados relevantes e precisos com base nos termos inseridos pelos usuários.
- **Sugestões de Pesquisa e Filtros**: Avaliamos a funcionalidade de sugestões de pesquisa e a capacidade de aplicar filtros avançados ou refinamentos de busca.

#### Níveis de Criticidade de Defeitos:

- **Baixa**: Defeitos que têm pouco impacto na usabilidade geral do site, como discrepâncias menores na exibição dos resultados da busca.
- **Média**: Defeitos que afetam parcialmente a funcionalidade da barra de busca, como sugestões de pesquisa imprecisas.
- **Alta**: Defeitos que impedem significativamente o uso da barra de busca, como falha total na funcionalidade de sugestões ou resultados de busca incorretos.

#### Resultados e Ações:

Após conduzirmos os testes da barra de busca de itens, documentamos nossas descobertas e recomendamos ajustes para melhorar a precisão dos resultados da busca e aprimorar a experiência do usuário durante a navegação pelo site.

#### Conclusão:

O Exploratory Testing nos permitiu identificar potenciais problemas na barra de busca de itens do site da Casa & Video. Essa abordagem flexível é baseada na experiência e será essencial para garantir a qualidade e a usabilidade do sistema, contribuindo para uma melhor experiência do usuário e maior satisfação ao realizar buscas por produtos no site.


<br/>
<table>
    <tr>
        <th>
            Objetivo
        </th>
        <th colspan="4">
            Verificar os itens buscados serão precisos
        </th>
    </tr>
    <tr>
        <th>
            Técnica:
        </th>
        <th colspan="2">
            ( ) manual
        </th>
        <th colspan="2">
            (x) automática
        </th>
    </tr>
    <tr>
        <th>
            Estágio do teste
        </th>
        <th>
            Integração ( )
        </th>
        <th>
            Sistema (x)
        </th>
        <th>
            Unidade ( )
        </th>
        <th>
            Aceitação ( )
        </th>
    </tr>
    <tr>
        <th>
            Abordagem do teste
        </th>
        <th colspan="2">
            Caixa branca ( )
        </th>
        <th colspan="2">
            Caixa preta (x)
        </th>
    </tr>
    <tr>
        <th>
            Responsável(is)
        </th>
        <th colspan="4">
            João Victor Piumbini Cheroto
        </th>
    </tr>
</table>
<br/>


### 3.3 - Requisito 3: Itens por Categoria

#### Exploratory Testing:

Nosso grupo decidiu realizar o teste da ferramenta de itens por categoria no site da Casa & Video utilizando a técnica de Exploratory Testing. Essa abordagem de teste ad hoc nos permite explorar o sistema de forma livre, descobrindo possíveis defeitos e problemas que podem não ter sido identificados em testes formais.

#### Utilização da Técnica:

Ao acessar o site da Casa & Video, navegamos pela seção de categorias e selecionamos a categoria de TV e Smart TV. Em vez de seguir um roteiro de teste predefinido, utilizamos nossa experiência e conhecimento para explorar os itens listados nessa categoria.

#### Teste da Ferramenta de Itens por Categoria:

Durante nossa exploração, encontramos um resultado inesperado: um aspirador smart listado na categoria de TV e Smart TV. Essa discrepância levanta questões sobre a precisão e relevância dos resultados da ferramenta de itens por categoria.

#### Critérios de Teste:

- **Precisão dos Resultados**: Verificamos se os resultados exibidos na categoria de TV e Smart TV correspondiam aos produtos relevantes para essa categoria.
- **Relevância dos Itens**: Avaliamos se os itens listados estavam de acordo com a categoria selecionada e se eram pertinentes para os usuários interessados em produtos de TV e Smart TV.
- **Consistência Visual**: Verificamos se a apresentação dos itens seguia o padrão visual do restante do site.

#### Níveis de Criticidade de Defeitos:

- **Baixa**: Inconsistências menores nos resultados da categoria.
- **Média**: Presença frequente de itens irrelevantes na categoria.
- **Alta**: Presença constante de itens completamente fora do escopo da categoria, prejudicando a experiência do usuário.

#### Resultados e Ações:

Após identificarmos a presença do aspirador smart na categoria de TV e Smart TV, documentamos nossa descoberta e recomendamos uma revisão na lógica de classificação dos itens por categoria. 

#### Conclusão:

O teste de Exploratory Testing revelou uma discrepância significativa na ferramenta de itens por categoria do site da Casa & Video. Essa abordagem flexível e baseada na experiência nos permitiu identificar um problema potencial que pode afetar a usabilidade e a confiabilidade da plataforma. Essa descoberta destaca a importância de testes contínuos e abrangentes para garantir a qualidade do sistema.


<br/>
<table>
    <tr>
        <th>
            Objetivo
        </th>
        <th colspan="4">
            Verificar se a ferramenta de itens por categoria exibe resultados precisos.
        </th>
    </tr>
    <tr>
        <th>
            Técnica:
        </th>
        <th colspan="2">
            ( ) manual
        </th>
        <th colspan="2">
            (x) automática
        </th>
    </tr>
    <tr>
        <th>
            Estágio do teste
        </th>
        <th>
            Integração ( )
        </th>
        <th>
            Sistema ( )
        </th>
        <th>
            Unidade ( )
        </th>
        <th>
            Aceitação (x)
        </th>
    </tr>
    <tr>
        <th>
            Abordagem do teste
        </th>
        <th colspan="2">
            Caixa branca ( )
        </th>
        <th colspan="2">
            Caixa preta (x)
        </th>
    </tr>
    <tr>
        <th>
            Responsável(is)
        </th>
        <th colspan="4">
            Luiz Fernando Sacht
        </th>
    </tr>
</table>
<br/>

### 3.4 - Requisito 4: Cadastro por usuário

#### Teste de Unidade:

Nosso grupo optou por realizar o teste do requisito de Cadastro de Usuário no site da Casa & Video utilizando a técnica de Teste de Unidade. Esta abordagem nos permite verificar componentes individuais do sistema de forma isolada, garantindo que cada parte funcione conforme o esperado.

#### Técnica Utilizada:

- **Verificação dos Campos Obrigatórios**: Confirmamos se todos os campos obrigatórios do formulário de cadastro estão funcionando corretamente. Isso inclui validar se o nome completo, endereço de e-mail, senha e informações de contato são inseridos corretamente e se são necessários para concluir o cadastro.
- **Confirmação por E-mail**: Garantimos que o usuário receba uma confirmação por e-mail após o cadastro bem-sucedido. Isso envolve verificar se o sistema envia automaticamente um e-mail de confirmação para o endereço fornecido pelo usuário e se o conteúdo do e-mail é claro e informativo.

#### Níveis de Criticidade de Defeitos:

- **Baixa**: Inconsistências menores nos campos do formulário de cadastro, como validações de entrada ausentes.
- **Média**: Falha na entrega da confirmação por e-mail após o cadastro bem-sucedido.
- **Alta**: Incapacidade total de concluir o processo de cadastro devido a erros graves nos campos obrigatórios ou falha na entrega da confirmação por e-mail.

#### Resultados e Ações:

Após a realização dos testes de unidade para o Cadastro de Usuário, documentamos nossas descobertas e recomendamos as seguintes ações:
- Correção de quaisquer falhas ou inconsistências encontradas nos campos obrigatórios do formulário de cadastro.
- Verificação e correção de quaisquer problemas relacionados à entrega de e-mails de confirmação após o cadastro bem-sucedido.

#### Conclusão:

O teste de unidade do Cadastro de Usuário permite verificar a funcionalidade essencial do sistema, garantindo que os usuários possam se cadastrar com sucesso e receber confirmações por e-mail. Esta abordagem é crucial para garantir uma experiência de usuário fluida e confiável no site da Casa & Video.


<br/>
<table>
    <tr>
        <th>
            Objetivo
        </th>
        <th colspan="4">
            Verificar se o sistema permite que os Usuários se cadastrem no site fornecendo informações como: Nome completo, endereço de e-mail, senha e informações de contato.
        </th>
    </tr>
    <tr>
        <th>
            Técnica:
        </th>
        <th colspan="2">
            ( ) manual
        </th>
        <th colspan="2">
            (x) automática
        </th>
    </tr>
    <tr>
        <th>
            Estágio do teste
        </th>
        <th>
            Integração ( )
        </th>
        <th>
            Sistema ( )
        </th>
        <th>
            Unidade (x)
        </th>
        <th>
            Aceitação ( )
        </th>
    </tr>
    <tr>
        <th>
            Abordagem do teste
        </th>
        <th colspan="2">
            Caixa branca ( )
        </th>
        <th colspan="2">
            Caixa preta (x)
        </th>
    </tr>
    <tr>
        <th>
            Responsável(is)
        </th>
        <th colspan="4">
            Rodrigo da Cunha
        </th>
    </tr>
</table>
<br/>


### 3.5 - Animação

Para teste de funcionalidade (para games, principalmente, mas não somente).
Aqui deve-se verificar se as animações existentes no programa são disparadas quando devem e se seguem uma sequência lógica.
Se possível usar teste automatizado.

<br/>
<table>
    <tr>
        <th>
            Objetivo
        </th>
        <th colspan="4">
            descreva aqui o objetivo
        </th>
    </tr>
    <tr>
        <th>
            Técnica:
        </th>
        <th colspan="2">
            ( ) manual
        </th>
        <th colspan="2">
            ( ) automática
        </th>
    </tr>
    <tr>
        <th>
            Estágio do teste
        </th>
        <th>
            Integração ( )
        </th>
        <th>
            Sistema ( )
        </th>
        <th>
            Unidade ( )
        </th>
        <th>
            Aceitação ( )
        </th>
    </tr>
    <tr>
        <th>
            Abordagem do teste
        </th>
        <th colspan="2">
            Caixa branca ( )
        </th>
        <th colspan="2">
            Caixa preta ( )
        </th>
    </tr>
    <tr>
        <th>
            Responsável(is)
        </th>
        <th colspan="4">
            João Victor Piumbini Cheroto
        </th>
    </tr>
</table>
<br/>

## 4 - Recursos

Esta seção deve descrever os recursos humanos, de ambiente de teste (hardware e software) e de ferramentas de automatização de testes necessários para execução dos testes que devem ser descritos nas subseções que seguem.

### 4.1 - Ambiente de teste - Software e Hardware

Descreva aqui o hardware e sua configuração, e o software. Por exemplo, o sistema operacional, browsers, servidor web, etc.
### 4.2 - Ferramenta de teste

Descreva aqui as ferramentas específicas de teste usadas no projeto.


## 5 - Integrantes

Alunos                      | Professora                       | Turma    | Matéria
----------------------------|----------------------------------|----------|--------------------------------------
João Victor Piumbini Cheroto|  Gabriela Martins de Jesus       | CC5N     | Qualidade e Testes de Software
Luiz Fernando Sacht         | Gabriela Martins de Jesus        | CC5N     | Qualidade e Testes de Software
Rodrigo da Cunha            |   Gabriela Martins de Jesus      | CC5N     | Qualidade e Testes de Software

