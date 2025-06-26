Este projeto é uma API RESTful completa desenvolvida em Java com Spring Boot 3 para gerenciar a autenticação e autorização de usuários usando JSON Web Tokens (JWT). A aplicação permite que novos usuários se registrem, façam login para obter um token de acesso e utilizem esse token para acessar rotas protegidas.

O projeto foi construído seguindo as melhores práticas de arquitetura de software, separando as responsabilidades em camadas (Controllers, Services, Repositories) e utilizando DTOs para a transferência de dados.

✨ Funcionalidades
Registro de Usuários: Endpoint público para a criação de novas contas de usuário.

Autenticação de Usuários: Endpoint público para login que, em caso de sucesso, retorna um token JWT.

Autorização via JWT: As rotas protegidas da API só podem ser acessadas com um token JWT válido no cabeçalho Authorization.

Validação e Geração de Token: Lógica de serviço para criar tokens com tempo de expiração e validar tokens recebidos.

Criptografia de Senhas: As senhas dos usuários são armazenadas de forma segura no banco de dados usando o algoritmo BCrypt.

Documentação da API: A API é documentada automaticamente com Springdoc (Swagger UI), fornecendo uma interface interativa para testar os endpoints.

Monitoramento: Métricas da aplicação são expostas via Spring Boot Actuator e prontas para serem consumidas pelo Prometheus.

Banco de Dados em Memória: Utiliza o H2 Database para facilitar o desenvolvimento e os testes sem a necessidade de configurar um banco de dados externo.

🛠️ Tecnologias Utilizadas
Java 17

Spring Boot 3

Spring Security

Spring Data JPA

Maven

JWT (JSON Web Token) - via biblioteca java-jwt da Auth0

Lombok

H2 Database

Springdoc OpenAPI (Swagger)

Spring Boot Actuator & Prometheus Micrometer
