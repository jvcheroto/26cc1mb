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
 |REQ-002    | Itens por categoria                                |
 |REQ-003    | Barra de busca                                     |
 
 
## 3 - Testes

Esta seção irá apresentar os testes escolhidos para cada iteração do projeto. Destacando a importância da seleção cuidadosa dos testes em cada iteração, este documento visa oferecer uma visão clara das abordagens adotadas para garantir a qualidade do software ao longo do desenvolvimento.

### 3.1 - Requisito: Itens de promoção

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



### 3.2 - Persistência de Dados

Para teste de integridade de dados e do banco de dados.
Aqui deve-se verificar se os dados não se perdem ao desligar o programa. Se o programa consegue se recuperar em caso de falha ou fechamento repentino.
Se possível usar teste automatizado.

<br/>
<table>
    <tr>
        <th>
            Objetivo
        </th>
        <th colspan="4">
            Verificar se dados são mantidos após súbito desligamento do programa .
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

### 3.3 - Integração dos Componentes

Para teste de funcionalidade.
Aqui deve-se verificar se as classes e métodos conseguem fazer a integração entre elas para uma sequência de ações do programa.
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
            (x) manual
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
            Integração (x)
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
            Caixa branca (x)
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

### 3.4 - Tempo de Resposta

Para teste de funcionalidade.
Aqui deve-se verificar se o tempo de respostas das ações do programa são consideradas aceitáveis.
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

