Endpoints(Get e Post)

-GET /Livros
Método: Get
URL: http://localhost:3000/livros
Body: Não tem
Resposta:
[
  {
    "id": 1,
    "titulo": "1984",
    "autor": "George Orwell"
  },
  {
    "id": 2,
    "titulo": "O Hobbit",
    "autor": "J.R.R. Tolkien"
  },
  {
    "id": 3,
    "titulo": "Dom Casmurro",
    "autor": "Machado de Assis"
  },
  {
    "id": 4,
    "titulo": "Harry Potter",
    "autor": "J.K. Rowling"
  },
  {
    "id": 5,
    "titulo": "Percy Jackson",
    "autor": "Rick Riordan"
  }
]


-Post /Livros
Método: Post
URL: http://localhost:3000/livros
Body:
{
  "titulo": "Nome do livro",
  "autor": "Nome do autor"
}

Resposta:
{
  "id": 1,
  "titulo": "Nome do livro",
  "autor": "Nome do autor"
}


-Exemplo de requisição no Postman
Configuração no Postman:
- Method: POST  
- URL: http://localhost:3000/livros  
- Body: Raw(JSON)
{
  "titulo": "1984",
  "autor": "George Orwell"
}

-Method: GET
- URL: http://localhost:3000/livros  
- Body: None
{
  "id": 1,
  "titulo": "1984",
  "autor": "George Orwell"
}

-Capturas de tela dos testes
Get:
<img width="1096" height="976" alt="image" src="https://github.com/user-attachments/assets/32e3e4b9-5660-4d60-8c4a-a1e2060394bf" />

Post:
<img width="1106" height="967" alt="image" src="https://github.com/user-attachments/assets/1d830faa-6dc6-4da1-bc4d-71e32fc3f552" />

Validação:
<img width="1116" height="867" alt="image" src="https://github.com/user-attachments/assets/00f3eab6-3260-46d1-85a1-ff5ac1aa1e7f" />


-Explicação de validações implementadas
O sinal de exclamação ! quer dizer "não" ou "vazio", que significa, "Se não existir título ou se não existir autor". Se a condição for verdadeira, ele interrompe a execução e envia o código HTTP 400 (Bad Request), que avisa o usuário que ele enviou algo errado.






