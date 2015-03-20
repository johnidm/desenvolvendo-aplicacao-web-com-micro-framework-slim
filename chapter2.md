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

Os método HTTP GET são mapeados atraves da função `get()`, vamos criar umaa rota que lista todas as cervejas:

$app->get('/cervejas', function () {

    echo 
    
});

Esse método é utilizado para listas todas as cervejas cadstradas no sistemas.

Observe que o primeiro paramtro da função `get`, `/cervejas` é recurso da URI.

Ao invocar a URI `htto://localhost:8080/cervejas` a função anonima passada no segundo parametro do methodo `get` e chamada e produz um resultado.

Voce pode observar que ao executar esse método o status de retorno doi 200 OK e no corpo do retorno HTTP, esta uma estrutura no formado JSON com todo as cervejas. Em métodos confirmado para retorno dados o corpo do HTTP é utilziad para isso, por exemplo se o retorno fosse quanquer outro formaro o copor seria utilziado para isso.


#### POST

Para os metodo HTTP POST utilizamos a finção `post`, veja o exemplo.

$app->post('/cerveja', function () {
    // Grava uma servija no DB
});

Aqui temos algo mais espeficico e internssnate, primeiro, estamos recupermdo o corpo do metho HTPP, isso é necessario pois o metodo POST é utilziado para criar recursos, dessa forma utilizamo ele para criar uma nova cevja. Obsere que as informaçõe da serveja devem ser passados no coropo da funcao.

Outro detalhe e que é uma boa pratica de provramalaoi devovloer o status 201 na resposta HTTP para o POST, pois estamos criadno ium recurso.


#### PUT 

Metodos do tipo PUT deve ser mapeados com a função `put()`, veja:

$app->put('/cerveja/:id', function ($id) {
    //Update book identified by $id
});

Observe que sua estrutura é muito pareceda com o POST, porem como po pUT e utilziado apra atualziar recursos, nos tmos que verificar se o recuso existe no DB caso contraro podemos retoanrdo um erro indcad que o resusto nao esta disponivel.


#### DELETE

O meto HTTP DELETE é utilizado para remover, excluir um recriso do DB, isso não significa exclui ele fiziamente, podemos por exemplo apenas flegar ele como excluido, 

$app->delete('/cerveja/:id', function ($id) {
    
});

Esse método e muit osemekhatne a GET porem é imporntae destaque que não ha necessidade de retorno de nenhuma informaçõe no coprot da função como o GET por eemplok, nesse caso é uma boa pratica rtorno o status 204 .









