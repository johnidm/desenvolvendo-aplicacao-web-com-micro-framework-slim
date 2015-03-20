# Slim Framework 



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






