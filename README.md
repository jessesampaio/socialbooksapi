Projeto SocialBooksAPI


Instruções e resumo:

--Banco de Dados H2
-Endereço: localhost:8080/h2-console

-Saved Settings: Generic H2 (Embedded)
-Saved Name: Generic H2 (Embedded)

-Driver Class: org.h2.Driver
-JDBC URL: jdbc:h2:mem:testdb
-User Name: sa
-Password:


--Endpoint (livros) 
http://localhost:8080/livros 
Descrição: Retorna todos os livros cadastrados. 
Método GET 

--Endpoint (livros/id) 
http://localhost:8080/livros/"id" 
Retorna o livro do id informado 
Método GET 

--Endpoint (livros) 
http://localhost:8080/livros 
Insere o livro do informado 
POST, raw, Json/Application 
{
	"nome" : "TDD em Java",
	"autor" : "Fulano",
	"editora" : "Escala"
}

--Endpoint (livros) 
http://localhost:8080/livros/id 
Atualiza um livro através do id informado 
PUT, raw, Json/Application 
{
	"nome" : "TDD em Java",
	"autor" : "Fulano",
	"editora" : "Escala"
}

--Endpoint (livros/id) 
http://localhost:8080/livros/"id" 
Deleta o livro do id informado 
Método DELETE



--Endpoint (autores)
http://localhost:8080/autores




--Conteúdo Principal

2. Criando uma API RESTful

-Criando o projeto
-Modelando nosso primeiro recurso
-Criando uma representação para o recurso Livro
-Utilizando a anotação @JsonInclude
-Interagindo com o banco de dados
-Salvando o recurso Livro a partir de um POST
-Buscando um livro com o uso da anotação @PathVariable
-Deletando o recurso Livro com o DELETE
-PUT para atualizar o recurso Livro
-Tratamento correto das respostas HTTP 404 e 201
-Finalizando o tratamento das respostas
-Melhorando o design do nosso código
-Manipulando erros com @ExceptionHandler e @ControllerAdvice
-Adicionando comentários ao recurso Livro
-Listando os comentários do recurso Livro
-Adicionando o recurso Autor à nossa API
-Evoluindo nosso recurso Autor
-Testando nossos recursos e formatando nossas representações JSON
-Validando as entradas na nossa API
-Negociação de conteúdos com Media Type


3. Refinando a API
Adicionando cache
Autenticação com Spring Security

4. Consumindo nossa API
Automatizando testes com Postman
Cliente Java
Evoluindo nosso cliente Java
Finalizando nosso cliente Java
Cliente JavaScript
Cross-Origin Resource Sharing (CORS)
Conclusão