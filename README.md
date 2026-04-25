# 🚀 Spring Boot User Management API

A production-ready RESTful API built using Spring Boot that performs full CRUD (Create, Read, Update, Delete) operations on users.

---

## 📌 Features

- Create new users
- Get all users
- Get user by ID
- Update user details
- Delete users
- Exception handling
- Clean layered architecture (Controller → Service → Repository)
- In-memory H2 Database
- RESTful API design

---

## 🧠 Tech Stack

- Java 17+
- Spring Boot
- Spring Web
- Spring Data JPA
- H2 Database
- Maven

---

## 📁 Project Structure
```
springboot-user-api/
│── src/
│ ├── main/
│ │ ├── java/com/example/demo/
│ │ │ ├── controller/
│ │ │ ├── service/
│ │ │ ├── repository/
│ │ │ ├── model/
│ │ │ ├── exception/
│ │ │ └── DemoApplication.java
│ │ └── resources/
│ │ └── application.properties
│
│── pom.xml
│── README.md
```

---

## ⚙️ Setup & Installation

### 1. Clone the Repository
```
git clone https://github.com/your-username/springboot-user-api.git

cd springboot-user-api
```

### 2. Run the Application
```
mvn spring-boot:run
```

### 3. App URL
```
http://localhost:8080
```

---

## 🗄️ H2 Database Console
```
http://localhost:8080/h2-console
```

Credentials:
```
JDBC URL: jdbc:h2:mem:testdb
Username: sa
Password: (leave empty)
```

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|--------|---------|------------|
| GET    | /api/users        | Get all users |
| GET    | /api/users/{id}   | Get user by ID |
| POST   | /api/users        | Create new user |
| PUT    | /api/users/{id}   | Update user |
| DELETE | /api/users/{id}   | Delete user |

---

## 🧪 Sample JSON
```
{
"name": "Rishi",
"email": "rishi@email.com
"
}
```

---

## 🧪 cURL Commands

### Create User
```
curl -X POST http://localhost:8080/api/users

-H "Content-Type: application/json"
-d '{"name":"Rishi","email":"rishi@email.com
"}'
```

### Get All Users
```
curl http://localhost:8080/api/users
```

### Update User
```
curl -X PUT http://localhost:8080/api/users/1

-H "Content-Type: application/json"
-d '{"name":"Updated","email":"updated@email.com
"}'
```

### Delete User
```
curl -X DELETE http://localhost:8080/api/users/1
```

---

## ⚠️ Error Handling

- 404 - User not found
- 500 - Internal server error

---

## 💡 Future Improvements

- JWT Authentication
- MySQL/PostgreSQL integration
- Pagination & filtering
- Swagger API documentation
- Docker support

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

---

## 📄 License

This project is licensed under the MIT License.

---

## 🌟 Support

If you like this project, give it a ⭐ on GitHub!
