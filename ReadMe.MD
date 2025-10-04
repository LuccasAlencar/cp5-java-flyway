# Sistema de Cadastro de Produtos

**Aluno:** Luccas de Alencar Rufino
**RM:** 558253

Este projeto foi desenvolvido para o Checkpoint 5 (CP5) da disciplina de Java Avançado. Trata-se de uma API REST para cadastro de produtos, utilizando Spring Boot, JPA e Flyway para controle de versão do banco de dados.

## Como rodar
Navegue até a pasta do projeto no terminal e rode os comandos:

mvn clean install
mvn spring-boot:run

depois só acessar: `http://localhost:8080/api/produtos`

## Endpoints

- `GET /api/produtos` - Lista todos os produtos
- `GET /api/produtos/{id}` - Busca um produto pelo ID
- `POST /api/produtos` - Cria um novo produto
- `DELETE /api/produtos/{id}` - Exclui um produto pelo ID

## Exemplo de Uso

### Criar um produto (POST)

Envie uma requisição POST para `http://localhost:8080/api/produtos` com o seguinte corpo (JSON):

```json
{
  "name": "Tablet",
  "price": 299.99,
  "category": "Eletrônicos"
}
