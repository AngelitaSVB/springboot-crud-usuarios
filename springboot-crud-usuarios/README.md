# 🚀 CRUD de Usuários com Spring Boot

Este projeto é uma API REST simples para gerenciamento de usuários, desenvolvida com **Java + Spring Boot** e **banco de dados H2 em memória**. Ideal para estudos de back-end e prática com operações CRUD (Create, Read, Update, Delete).

---

## 🔧 Tecnologias utilizadas

- Java 17
- Spring Boot 3.2.5
- Spring Web
- Spring Data JPA
- H2 Database
- Maven

---

## 📁 Endpoints da API

| Método | Endpoint             | Descrição                   |
|--------|----------------------|-----------------------------|
| POST   | `/usuarios`          | Cadastra um novo usuário    |
| GET    | `/usuarios`          | Lista todos os usuários     |
| PUT    | `/usuarios/{id}`     | Atualiza os dados do usuário|
| DELETE | `/usuarios/{id}`     | Remove um usuário do sistema|

---

## 🧪 Como testar a API

Você pode usar ferramentas como [Insomnia](https://insomnia.rest/) ou [Postman] para testar os endpoints.  

### ▶️ Criar usuário (POST)

```http
POST http://localhost:8080/usuarios
Content-Type: application/json
```

```json
{
  "nome": "Angelita",
  "email": "angelita@email.com"
}
```

---

### 📥 Listar usuários (GET)

```http
GET http://localhost:8080/usuarios
```

---

### ✏️ Atualizar usuário (PUT)

```http
PUT http://localhost:8080/usuarios/1
Content-Type: application/json
```

```json
{
  "nome": "Angelita Atualizada",
  "email": "nova@email.com"
}
```

---

### ❌ Deletar usuário (DELETE)

```http
DELETE http://localhost:8080/usuarios/1
```

---

## 💻 Como rodar o projeto localmente

1. Clone o repositório:

```bash
git clone https://github.com/AngelitaSVB/springboot-crud-usuarios.git
cd springboot-crud-usuarios
```

2. Rode o projeto com Maven:

```bash
mvn spring-boot:run
```

3. Acesse no navegador:

- API: `http://localhost:8080/usuarios`
- Console H2: `http://localhost:8080/h2-console`  
  - JDBC URL: `jdbc:h2:mem:usuarios`  
  - Usuário: `sa`  
  - Senha: *(deixe em branco)*

---

## 📝 Observações

- O banco de dados H2 é **em memória**, ou seja, os dados são apagados ao reiniciar o projeto.
- Este projeto é ideal para aprendizado, demonstração de APIs REST e integração com front-ends ou ferramentas de testes.

---

## 👩‍💻 Autora

Desenvolvido por **Angelita da Silva Vilas Boas**  
📚 Estudante de Ciência de Dados | Back-End | Java | Python | AWS  
🔗 [LinkedIn](https://www.linkedin.com/in/angelitasvb)
