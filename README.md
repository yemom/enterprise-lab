[![CI](https://github.com/yemom/enterprise-lab/actions/workflows/main.yml/badge.svg)](https://github.com/yemom/enterprise-lab/actions/workflows/main.yml)

# Enterprise Lab - Product Service API (Lab 2)

Spring Boot RESTful Product Catalogue API implementation.

## Setup Instructions

1. Clone this repository.
2. Open a terminal in the project root.
3. Move to the Maven module:

```bash
cd demo
```

4. Start the API:

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

- postman/product-service-lab2.json

## Tests

From the demo folder:

```bash
mvn test
```

Current status: 11 tests run, 0 failures.
