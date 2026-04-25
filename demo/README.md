[![CI](https://github.com/yemom/enterprise-lab/actions/workflows/main.yml/badge.svg)](https://github.com/yemom/enterprise-lab/actions/workflows/main.yml)

    Name                ID
Esrom Basazinaw    ATE/5227/14
Yohanes Seyum      ATE/5195/14

# Product Service API (Lab 2)

RESTful Product Catalogue API built with Spring Boot.

## Setup Instructions

1. Clone the repository.
2. Move into the project module:

```bash
cd demo
```

3. Run the application:

```bash
mvn spring-boot:run
```

Base URL:

- http://localhost:8082/api/v1/products

## Swagger

- Swagger UI: http://localhost:8082/swagger-ui.html
- OpenAPI JSON: http://localhost:8082/api-docs

## API Endpoints (All 5 CRUD)

| Method | Endpoint | Description |
|---|---|---|
| GET | /api/v1/products | List all products |
| GET | /api/v1/products/{id} | Get product by ID |
| POST | /api/v1/products | Create a product |
| PUT | /api/v1/products/{id} | Update a product |
| DELETE | /api/v1/products/{id} | Delete a product |

## Postman Collection

- Required file path: postman/product-service-lab2.json

## Tests

Run all tests:

```bash
mvn test
```

Current suite includes positive and negative scenarios for:

- CRUD status codes
- Validation errors (400 ProblemDetail)
- Unknown resource errors (404 ProblemDetail)
