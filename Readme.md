🛒 E-Commerce Platform (Spring Boot)
A full-featured E-Commerce Web Application built using Spring Boot (Java) that supports product browsing, cart management, secure checkout, and admin management features.
🚀 Features
👤 User Features
Register, Login, and Logout (Spring Security + JWT)
Browse products by category
Search and filter products
Add to Cart / Remove from Cart
Checkout and place orders
View order history and details
🧑‍💼 Admin Features
Manage products (Add, Edit, Delete)
Manage categories
Manage users and orders
Dashboard with sales statistics
⚙️ Technical Features
RESTful API (Spring Boot)
JPA/Hibernate for ORM
MySQL/PostgreSQL database integration
Exception Handling and Validation
Unit & Integration Testing
Swagger API documentation
🧱 Tech Stack
Layer	Technology
Backend	Spring Boot 3+, Spring Web, Spring Data JPA, Spring Security
Database	MySQL / PostgreSQL
Authentication	JWT (JSON Web Tokens)
Build Tool	Maven or Gradle
Documentation	Swagger / OpenAPI
Testing	JUnit, Mockito
Frontend (optional)	React / Angular / Thymeleaf
📁 Project Structure
ecommerce-springboot/
│
├── src/
│   ├── main/
│   │   ├── java/com/example/ecommerce/
│   │   │   ├── controller/        # REST Controllers
│   │   │   ├── model/             # Entity Classes
│   │   │   ├── repository/        # JPA Repositories
│   │   │   ├── service/           # Business Logic
│   │   │   ├── security/          # JWT & Config
│   │   │   └── EcommerceApplication.java
│   │   └── resources/
│   │       ├── application.yml    # Configuration
│   │       ├── data.sql           # Sample Data
│   │       └── schema.sql         # DB Schema
│   └── test/
│       └── ...                    # Unit Tests
│
├── pom.xml                        # Maven Dependencies
└── README.md
⚙️ Setup & Installation
1️⃣ Prerequisites
Make sure you have installed:
Java 17+
Maven 3.9+
MySQL or PostgreSQL
2️⃣ Clone the Repository
git clone https://github.com/your-username/ecommerce-springboot.git
cd ecommerce-springboot
3️⃣ Configure Database
Edit src/main/resources/application.yml:
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/ecommerce_db
    username: root
    password: yourpassword
  jpa:
    hibernate:
      ddl-auto: update
    show-sql: true
  security:
    jwt:
      secret: your_secret_key
4️⃣ Build and Run
mvn clean install
mvn spring-boot:run
5️⃣ Access the Application
API Base URL: http://localhost:8080/api
Swagger Docs: http://localhost:8080/swagger-ui.html
