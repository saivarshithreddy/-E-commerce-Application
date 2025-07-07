# E-commerce/Library Full Stack Application

A modern full-stack web application for managing a library or e-commerce platform. Built with **React** (frontend) and **Spring Boot** (backend), featuring secure authentication, REST APIs, MySQL integration, and Stripe payments.

---

## 🚀 Features

- User authentication with Okta (OAuth2/OIDC & JWT)
- Book browsing, checkout, and review system
- Admin panel for managing books and messages
- Secure RESTful API with Spring Boot
- MySQL database integration
- Stripe payment processing
- Responsive UI with React, Bootstrap

---

## 🛠️ Tech Stack

**Frontend:**
- React (TypeScript)
- React Router
- Axios/Fetch
- Bootstrap
- Okta Auth

**Backend:**
- Spring Boot (Java 18)
- Spring Security (JWT, OAuth2)
- Spring Data JPA
- MySQL
- Stripe API
- Maven

---

## 📁 Project Structure

```
- backend/
  └── spring-boot-library/
      └── spring-boot-library/  # Java Spring Boot app (API, security, DB)
- frontend/
  └── react-library/           # React app (UI, routing, API calls)
```

---

## ⚙️ Setup & Usage

### 1. Clone the Repository
```bash
git clone <your-repo-url>
cd -E-commerce-Application
```

### 2. Backend Setup (Spring Boot)
```bash
cd backend/spring-boot-library/spring-boot-library
# Configure MySQL in src/main/resources/application.properties
# Example:
spring.datasource.url=jdbc:mysql://localhost:3306/your_db
spring.datasource.username=your_user
spring.datasource.password=your_password

# Run with Maven
./mvnw spring-boot:run
```

### 3. Frontend Setup (React)
```bash
cd ../../../frontend/react-library
npm install
npm start
# App runs at http://localhost:3000
```

### 4. Environment Variables
- **Backend:** Set MySQL credentials and Stripe keys in `application.properties`.
- **Frontend:** Configure Okta settings in `.env` or directly in the code (see Okta docs).

---

## 🧪 Testing
- **Backend:**
  - `./mvnw test`
- **Frontend:**
  - `npm test`

---

## 📦 Deployment
- Build backend: `./mvnw package`
- Build frontend: `npm run build`
- Deploy as needed (Docker, cloud, etc.)

---

## 🤝 Contributing
1. Fork the repo
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit and push
4. Open a Pull Request
