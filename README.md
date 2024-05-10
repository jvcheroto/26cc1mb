# Plano de Teste

**CASA & VIDEO**

# Sobre Casa & Video

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
 |REQ-001    | Barra de busca                                     |
 |REQ-002    | Itens por categoria                                |
 |REQ-003    | Itens de promoção                                  |
 
 
## 3 - Testes

Esta seção irá apresentar os testes escolhidos para cada iteração do projeto. Destacando a importância da seleção cuidadosa dos testes em cada iteração, este documento visa oferecer uma visão clara das abordagens adotadas para garantir a qualidade do software ao longo do desenvolvimento.

### 3.1 - Requisito: Itens de promoção

Durante o teste do sistema no site da Casa & Video, uma discrepância nos preços dos produtos foi identificada durante o processo de finalização da compra. Enquanto o produto estava em promoção no site por R$ 289,90, ao ser adicionado ao carrinho com a aplicação de um cupom de desconto e a escolha do método de pagamento via Pix, o preço final aumentou para R$ 336,18. Essa divergência entre os valores levanta questões sobre a integridade e precisão do sistema de precificação da plataforma, assim como a experiência do usuário durante a compra. 

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

