# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth já configurada, feita para ser usada no desenvolvimento das API's nos Capstones do Q2.

## Endpoints

Assim como a documentação do JSON-Server-Auth traz (https://www.npmjs.com/package/json-server-auth), existem 3 endpoints que podem ser utilizados para cadastro e 2 endpoints que podem ser usados para login.

### Cadastro

POST /register <br/>
POST /signup <br/>
POST /users

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.


### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"

### Atualizar Usuario
PUT /users/id(id do usuario)

email e senha são obrigatórios!!!

{
		"email": "kenzinho@mail.com",
	"password":"1234567",
		"name": "Adriano",
		"age": 38,
		"id": 1
	}
  
  


### Cadastro de Produtos

POST /product
É preciso passar o userId do usuario (como explica na documentação da API - https://www.npmjs.com/package/json-server-auth) para poder cadastrar o produto.

{
      "name": "Tapete Higiênico Super Me.Au Pet para Cães",
      "description": "Tapete Higiênico Super Me.Au Pet: Alegria em forma de produtos de qualidade, que te ajudam a economizar tempo e dinheiro.",
      "price": 67.15,
      "type": "Higiene",
      "img": "https://www.petlove.com.br/images/products/251757/product/Bowl_Future_Pet_para_C%C3%A3es_e_Gatos_-_800_mL_2765001_%281%29.jpg?1642454399",
      "petType": "Todos",
      "userId": 4,
      "id": 2
    }

### Atualização de algum dado do Produto
PUT /product/id(id do produto)

É preciso passar o userId do usuario (como explica na documentação da API - https://www.npmjs.com/package/json-server-auth) para poder cadastrar o produto.


### Deletar um produto

DELETE /product/id(id do produto)





