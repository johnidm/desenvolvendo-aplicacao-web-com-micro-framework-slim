# Slim Framework 

Quando falamos em frameworks para desenvolvimento de software temos a disposição, na maiorias das vezes, de caracteriticas que provem suporte para resolver um conjunto de problemas, por exemplo: vamos criar um sistemas de e-commerce, nós temos a disposição vários frameoworks que provem uma serie de funções, classes, bibliotecas e ferrametnas que dão suporte a criação do e-commerce.

Basicamente podemos definir que é um conjunto de funcoes que se relacionam entre si a fim de dar sustentação a contruão de algo maior que possui outras exigencias que o framwork em si nao se propoe a resolver, utilizando o exemplo do e-commerce, em si o framework escolhido nao fazer vendas na internet, mas prove uma serie de fatures que possibilitam a contrução de um produto que faça vendas na internet. 

Você podem perceber que frameworks nos oferencem possibildaide de reuso de cópdigo, estrutura padronizadas, o que nos permite criar aplicações de forma elegante e rapida, e exigindo uma cruva de aprendizado relativamente grande.


O Slim é classificado em uma categoria muito interessante conhecido com micro frameworks, que provem funcionalidades mais especificar, possuem facil instalação, e exigem uma curva de apresndizado menor, consequantemente menos código e mais facil a manutençao e escrita desse projetos, porem a sua abrangencia é menor pois muitas vezes se limitam a resolover problemas mais especificos.

O PHP possui inumeros micro frameworks, outras lingagens de programação com o Python e Ruby tambem possuem micro frameworks.

O Slim é um micro framework para utilziado para desenvovler aplicações Web e API, ao longo desse e-book nos vamos demonstrar todo esse poder e simplicidade, integrando o Slim com outros framework a fim de ter um econssistema que permite desenvover projetos urpreendentes e elegantes.

~~Falar das principais funcionaldiade do Slim~~

### Methos HTTP

~~Falar sobre os métodos HTTP e a estrutura dos métodos~~

~~Tabela com as convenções adotadas nos métodos HTTP~~

```
GET    | /clientes      | 200 OK
GET    | /cliente/{id}  | 200 OK
POST   | /cliente       | 201 Created
PUT    | /cliente/{id}  | 204 Not Content
DELETE | /cliente/{id}  | 204 Not Content
```

Para os métodos PUT e POST o `body` da requisição deve ter dados para serem tratados no servidor.

No método POST, no `header` da resposta da requisição é enviado no campo `Location` um URI com o novo recurso criado. Exemplo: `http://localhost:8000/cliente/12`.






