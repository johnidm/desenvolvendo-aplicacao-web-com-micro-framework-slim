# Slim Framework 

Quando falamos em frameworks para desenvolvimento de software temos a disposição um conjunto, na maiorias das vezes, de caracteriticas que provem suporte para resolver um conjunto de problemas, por exemplo: vamos criar um sistemas de e-commerce, nós temos a disposição vários frameoworks que provem uma serie de funções, classes bibliotecas que dão suporte a criação do e-commerce, facilitando o resuso de código e oferencendo uma padronizada.


, em PHP os framework são econssistemas  que nos dão a capacidade de criar aplicações de uma forma elegante e rapida

temos a disposição inumeras ferramentas e possibilidade de estrturas com uma curva de apresndizado relativametne dificil, e com inumeras configução e muito código oque certamente ao final nos da um podemo enorme para criar projetos. 

BAsicamente podemos definir que é um conjunto de funcoes que se relacionado a fim de dar sustentação a contruão de algo maior de outras exigencias que o framwork nao corresponde.

NO geral um framework e um estrutura que serve de apior para o desenvolvimento de algim mais especifico, em muitos casos eles fornecem estrutura de cadas que se relacionam e especificam como devemos crontruir nosso projetos. 


O Slim é classificado em uma categoria muito interessante conhecido com micro frameworks, que provem funcionalidades mais especificar com a caracteritia de serem facies de se traalhar e que exigem uma curva de apresndizado menor,  com boa prerformance.

O PHP possui inumeros micro frameworks, outras lingagens de programação com o Python e Ruby tambem possuem micro frameworks.




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






