# JWT Authentication Login/Register Application  

![Java](https://img.shields.io/badge/Java-21-007396?style=for-the-badge&logo=java)  
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.1.2-brightgreen?style=for-the-badge&logo=spring)  
![Maven](https://img.shields.io/badge/Maven-4.0.0-C71A36?style=for-the-badge&logo=apache-maven)  
![H2 Database](https://img.shields.io/badge/H2%20Database-In%20Memory%20Database-blue?style=for-the-badge&logo=h2)  
![JUnit](https://img.shields.io/badge/Testing-JUnit5-yellowgreen?style=for-the-badge&logo=java)  

A robust JWT Authentication system built using Spring Boot (Java 21) and Maven. It includes features for **user registration**, **login**, and **authentication** with JWT. This project also contains unit tests for backend functionalities, an embedded H2 database, and simple HTML pages for testing registration and login functionalities.  

---

## 📑 Features  

1. **User Registration**:  
   - Create new accounts with a secure password.  
2. **Login Functionality**:  
   - Authenticate users using email and password.  
3. **JWT Authentication**:  
   - JSON Web Tokens for secure API access and session management.  
4. **Unit Tests**:  
   - Comprehensive backend unit tests using JUnit 5.  
5. **H2 Database**:  
   - In-memory database for testing and development purposes.  
6. **Frontend HTML Pages**:  
   - Test register and login functionalities via basic HTML pages.  

---

## 🚀 Technology Stack  

- **Backend**: Spring Boot (Java 21)  
- **Frontend**: Simple HTML  
- **Database**: H2 Database (in-memory)  
- **Build Tool**: Maven  
- **Testing**: JUnit 5  

---

## 📂 Project Structure
    src/main/java 
    ├── com.authentication.authentication
    │    ├── config // Spring Security and JWT Configuration 
    │    ├── controller // REST Controllers for Authentication 
    │    ├── model // Entity Models (e.g., User)
    │    ├── repository // Repositories (e.g., UserRepository) 
    │    ├── service // Business Logic (e.g., AuthenticationService) 
    │    └── utils // Helper classes for JWT creation and validation
    └──...

    src/main/resources
    ├── static // CSS file
    ├── templates // HTML pages for testing register and login 
    ├── application.properties // App configurations

    src/test/java 
    ├── com.authentication.authentication // Unit Tests

---

## 🛠️ Prerequisites  

- Java 21  
- Maven 4.0+  
- IDE (e.g., IntelliJ IDEA, Eclipse)  

---

## ⚙️ Installation  

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/barispinara/jwt_authentication_springboot.git
   cd jwt_authentication_springboot/authentication
2. **Build the Project**
    ```bash
    mvn clean install
3. **Run the Application**
    ```bash
    mvn spring-boot:run
4. **Access the Application**
    - Open a browser and navigate to `https://localhost:8080`

## 📄 API Endpoints  

| **Endpoint**          | **Method** | **Description**          | **Protected** |  
|------------------------|------------|--------------------------|---------------|  
| `/user/register`           | `POST`    | Register a new user      | Yes            |  
| `/user/login`              | `POST`    | Login and get JWT token  | Yes            |  
| `/home`    | `GET`     | Homepage of the project       | No           |
| `/register`    | `GET`     | Register page  of the project       | No           |
| `/`    | `GET`     | Login page of the project       | No           |


## 🛠️ Testing

1. **Unit Tests**


    Run all backend unit tests:
    ```bash
    mvn test
2. **Manual Testing**


    After running the project, you can test the project manually from `https://localhost:8080`
## 🔧 Configuration  

### H2 Database Console  

The application uses an in-memory H2 database. You can access the H2 console at:  

- **URL**: [http://localhost:8080/h2-console](http://localhost:8080/h2-console)  
- **Default Credentials**:  
  - **JDBC URL**: `jdbc:h2:file:./.data/h2`  
  - **Username**: `admin`  
  - **Password**: *12345*  

## 🔧 JWT Configuration  

Modify JWT expiration time and secret in the `application.properties` file:

    
    jwt.secret=your-secret-key
    jwt.expiration=3600000

## 🧪 Unit Test Coverage

The project includes unit tests to validate critical functionalities like user registration, login, and JWT validation.

## 📧 Contact

Feel free to reach out for suggestions or contributions from github issues or PR

