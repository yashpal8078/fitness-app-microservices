# Fitness App Microservices

A comprehensive **Microservices-based Fitness Application** built using Java Spring Boot, Spring Cloud services, and a modern frontend. This project demonstrates real-world design and implementation of a distributed system where each service is responsible for a specific domain of functionality — such as user management, activity tracking, gateway routing, service discovery, and frontend UI.

---

## 🚀 Overview

This project showcases how to build a scalable fitness platform using a microservices architecture.

Microservices provide:

- Modular development with independently deployable services  
- Better scalability and fault isolation  
- A real-world structure that mirrors enterprise applications using Spring Boot and Spring Cloud principles  

---

## 📦 Project Structure



```text
fitness-app-microservices/
├── activityservice/     # Domain: Activity logging & metrics
├── aiservice/           # Domain: AI-powered fitness recommendations
├── userservice/         # Domain: Profile management & Auth
├── configserver/        # Infrastructure: Centralized YAML/Properties
├── eureka/              # Infrastructure: Service Registration
├── gateway/             # Infrastructure: Routing & Security
└── fitness-app-frontend/# UI: React.js Dashboard

Each folder represents a separate module or service in the system.


---

## 🛠️ Technologies Used

| Category | Technologies |
|---------|--------------|
| Backend | Java, Spring Boot, Spring Cloud |
| Service Discovery | Eureka |
| API Routing | Spring Cloud Gateway |
| Configuration | Spring Cloud Config |
| Frontend | React |
| Build Tool | Maven |
| Communication | REST APIs |



---

## 📌 Key Features

✔ Independent microservices for different domains  
✔ API Gateway for unified entry point  
✔ Centralized configuration management  
✔ Service discovery for dynamic routing  
✔ Modular and maintainable code structure  

---

## 📋 Getting Started

### Prerequisites

Make sure you have installed:

- Java 11+  
- Maven  
- Node.js  
- Git  

---

## 🧱 Backend Setup

1. Open backend services in **IntelliJ**
2. Navigate to each service folder  
3. Build and run:

```bash
mvn clean install
mvn spring-boot:run
Recommended Startup Order
nginx
Copy code
configserver → eureka → gateway → userservice → activityservice → aiservice
🖥️ Frontend Setup
Open fitness-app-frontend in VS Code

Install dependencies:

bash
Copy code
npm install
Start development server:

bash
Copy code
npm start
🧪 Testing
Run backend tests using:

bash
Copy code
mvn test
📁 Environment Configuration
For local development, create .env files under respective folders if required.

Example:

ini
Copy code
API_GATEWAY=http://localhost:8080
USER_SERVICE=http://localhost:8081
📌 Notes
Designed as an educational project to demonstrate microservices architecture.

Suitable for use as a portfolio project or learning reference.

📜 License
This project is shared for learning purposes.

🙏 Credits
This project was built as part of a microservices learning track focused on real-world Spring Boot applications.
