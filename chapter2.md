# Slim Framework 

Quando falamos em frameworks para desenvolvimento de software temos a disposição, na maiorias das vezes, de caracteriticas que provem suporte para resolver um conjunto de problemas, por exemplo: vamos criar um sistemas de e-commerce, nós temos a disposição vários frameoworks que provem uma serie de funções, classes, bibliotecas e ferrametnas que dão suporte a criação do e-commerce.

Basicamente podemos definir que é um conjunto de funcoes que se relacionam entre si a fim de dar sustentação a contruão de algo maior que possui outras exigencias que o framwork em si nao se propoe a resolver, utilizando o exemplo do e-commerce, em si o framework escolhido nao fazer vendas na internet, mas prove uma serie de fatures que possibilitam a contrução de um produto que faça vendas na internet. 

Você podem perceber que frameworks nos oferencem possibildaide de reuso de cópdigo, estrutura padronizadas, o que nos permite criar aplicações de forma elegante e rapida, e exigindo uma cruva de aprendizado relativamente grande.


O Slim é classificado em uma categoria muito interessante conhecido com micro frameworks, que provem funcionalidades mais especificar, possuem facil instalação, e exigem uma curva de apresndizado menor, consequantemente menos código e mais facil a manutençao e escrita desse projetos, porem a sua abrangencia é menor pois muitas vezes se limitam a resolover problemas mais especificos.

O PHP possui inumeros micro frameworks, outras lingagens de programação com o Python e Ruby tambem possuem micro frameworks.

O Slim é um micro framework para utilziado para desenvovler aplicações Web e API, ao longo desse e-book nos vamos demonstrar todo esse poder e simplicidade, integrando o Slim com outros framework a fim de ter um econssistema que permite desenvover projetos urpreendentes e elegantes.

### Postman



### Methos HTTP

### Rotas

Esse provalemente é o rescuros mais interssante do Slim, a construção de rotas, se você esta familiarizado com framework como AngularJS ou Play FRamework, sabe que esse recurso é muito uitil, quando utilizandos framework baseados em actions conseguimos criar um esquema de roteamento bem organizado, veja o exemplo:

ao acessar a URL `htto://localhost/produtos` no browser temos uma rota que esta direciando nossa navegação para o recurso `produtos` vinculado ao method HTTP GET, pelo fato de termos acessado pelo brwoser, que esse recurso `produtos` faz? Isso depende, podemos ter nesse recurso uma API que devove uma resposta ao clente, o broweser, uma lista de produto no formado JSON ou XML, ou em outro caso o terorno de uma página html rednerizad para lista os produtos de uma base de dados pro exemplo.

O que é interssante oberver é que as rotas sçao definidas no nosso istemas para acesar recursos, esse recursos nos deveolver respostas, todos o funcimanteo de rotas no Slim objeced esse fluxo, de requisição e resposta. 

O correto entendimento de Methos HTTP é importante par entender as rotas.

Com o Slim nos podemos fazer um mapeamento de rotas, URI, com funcões que especifica com isso nos temso uma facilidade de criar em consumir recursos HTTP.

### Criando rotas

Nesse primeita parte vamos criar um mapa de rotas com o objetivo manipular em formato JSON cervejas em uma cervejaria. o formato JSON foi escolhido por ser de facill entendiento, mas podemos utilizar outros formatos como XML outr texto puro. Bastando apenas mudar o tipo dados trfegados on cabeçalhos das funções.

Caso uma rota não estevja mapeado o Slim retornar o código 404 - Not Found.

Crie um arquivo chamado rotas.php

#### GET 

Os método HTTP GET são mapeados atraves da função `get()`, veja:

$app->get('/books/:id', function ($id) {
    //Show book identified by $id
});




