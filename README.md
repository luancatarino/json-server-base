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

## Animals

POST/animals <br/>
GET/animals

Use o post para cadastrar um novo animal, precisa estar logado para cadastrar.
Ex: {
"type": "dog",
"name": "Simba",
"userId": 3,
}

Use o get para verificar os seus animais cadastrados, precisa estar logado para visualizar.

## Hobbie

POST/hobbies <br/>
GET/hobbies

Use o post para cadastrar um novo hobby, precisa estar logado para cadastrar.
Ex: {
"type": "reading",
"hoursSpent": 2,
"userId": 3,
}

Use o get para verificar os seus animais cadastrados, não é necessário estar logado.
