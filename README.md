# 🎓 StudentHub

A full-stack **Student Management System** built with **Spring Boot**, featuring secure authentication, student record management, and a clean Thymeleaf-powered UI.

---

## 🚀 Features

- **Student CRUD Operations** — Create, read, update, and delete student records
- **Spring Security** — Role-based authentication and authorization
- **Form Validation** — Input validation with helpful error messages
- **Thymeleaf Templates** — Server-side rendered HTML views
- **MySQL Database** — Persistent storage via Spring Data JPA
- **Hot Reload** — Spring Boot DevTools for faster development

---

## 🛠️ Tech Stack

| Layer       | Technology                          |
|-------------|--------------------------------------|
| Backend     | Java 11, Spring Boot 2.6.3           |
| Security    | Spring Security 5                    |
| Frontend    | Thymeleaf, HTML, CSS                 |
| Database    | MySQL, Spring Data JPA (Hibernate)   |
| Build Tool  | Maven                                |
| Dev Tools   | Spring Boot DevTools                 |

---

## 📁 Project Structure

```
studentHub/
├── src/
│   ├── main/
│   │   ├── java/          # Java source files (controllers, services, models)
│   │   └── resources/
│   │       ├── templates/ # Thymeleaf HTML templates
│   │       └── static/    # CSS, JS, images
│   └── test/              # Unit and integration tests
├── .mvn/wrapper/          # Maven wrapper
├── pom.xml                # Project dependencies
└── README.md
```

---

## ⚙️ Prerequisites

- **Java 11** or higher
- **Maven 3.6+** (or use the included `mvnw` wrapper)
- **MySQL 8+** running locally

---

## 🏁 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/thisisPremG/studentHub.git
cd studentHub
```

### 2. Configure the database

Create a MySQL database and update `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/studenthub_db
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### 3. Run the application

```bash
# Using Maven wrapper (no Maven installation needed)
./mvnw spring-boot:run

# Or on Windows
mvnw.cmd spring-boot:run
```

### 4. Open in browser

```
http://localhost:8080
```

---

## 🔐 Security

The application uses **Spring Security** for authentication. Default credentials can be configured in `application.properties` or via a custom `UserDetailsService`. Ensure you update default credentials before deploying to production.

---

## 🧪 Running Tests

```bash
./mvnw test
```

---

## 📦 Building for Production

```bash
./mvnw clean package
java -jar target/student-management-0.0.1-SNAPSHOT.jar
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

