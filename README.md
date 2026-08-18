# KLH-CSE-2026-27-2420030558-SmartCampus
# Smart Campus: Placement Management System

## Team Members

* **B. Kundana Mani** - 2420030558
* **M. Sai Kridhay Kumar** - 2420030211

## Supervisor

**Ms. R. Navyatha**

## Abstract

The **Smart Campus: Placement Management System** is a microservices-based application designed to simplify and manage the campus placement process for students, recruiters, and administrators. The system provides a centralized platform for managing student profiles, academic information, skills, company details, job opportunities, eligibility criteria, applications, interview schedules, and selection results.

The system allows students to create and maintain their profiles, view available job opportunities, check their eligibility, apply for suitable positions, and track their application status. Recruiters can manage company information, create job postings, define eligibility requirements, review applications, shortlist candidates, and update recruitment results. Administrators can manage users, companies, job postings, applications, and overall placement activities.

The project follows a **Service-Oriented Architecture using microservices**, where different placement functionalities are divided into independent services such as **Student Service, Company and Job Service, Application Service, and Notification Service**. The backend is developed using **Java, Spring Boot, and Spring Cloud**, with **PostgreSQL** used for data management. **Eureka Service Discovery** is used for service registration and discovery, while **Spring Cloud Gateway** manages API routing. **Spring Security and JWT** provide secure authentication and role-based authorization for students, recruiters, and administrators.

The system uses REST APIs for communication between services and provides a scalable and organized approach to placement management. Overall, the project aims to reduce manual effort, improve application tracking, simplify recruiter and student interactions, and provide a secure and efficient platform for managing the complete campus placement process.

## Setup and Execution

### 1. Install Required Tools

Install **Java JDK, Maven, Node.js, PostgreSQL, and Git**.

### 2. Clone the Repository

```bash
git clone https://github.com/kundanamani-23/KLH-CSE-2026-27-2420030558-SmartCampus
cd KLH-CSE-2026-27-2420030558-PlacementManagement
```

### 3. Configure PostgreSQL

Create the required databases for the microservices and configure the database credentials in the respective `application.properties` or `application.yml` files.

### 4. Start Eureka Server

Start the Eureka Service Discovery server first:

```bash
mvn spring-boot:run
```

### 5. Start the Microservices

Start the following services individually:

* Student Service
* Company & Job Service
* Application Service
* Notification Service

For each service:

```bash
mvn spring-boot:run
```

### 6. Start the API Gateway

Start the Spring Cloud Gateway:

```bash
mvn spring-boot:run
```

### 7. Start the Frontend

Navigate to the frontend directory:

```bash
npm install
npm run dev
```

### 8. Test the APIs

Use **Postman** to test the REST APIs, authentication, authorization, job postings, student applications, and other microservice operations.

## Project Features

* Student registration and profile management
* Company and recruiter management
* Job posting and eligibility management
* Student job applications
* Application status tracking
* Candidate shortlisting
* Interview status management
* Selection result management
* Notifications and updates
* JWT-based authentication
* Role-based authorization
* REST API-based communication
* Microservices-based architecture
* Service discovery using Eureka
* API routing using Spring Cloud Gateway
* Database per microservice

## Technologies Used

* Java
* Spring Boot
* Spring Cloud
* Spring Security
* JWT
* React
* PostgreSQL
* REST APIs
* Eureka Service Discovery
* Spring Cloud Gateway
* Docker
* GitHub Actions
* Postman

## Current Phase Status

* **Phase 1 – Project Selection & Planning:** Completed
* **Phase 2 – System Requirements & Architecture:** In Progress
* **Phase 3 – Microservice Development:** Not Started
* **Phase 4 – Frontend Development:** Not Started
* **Phase 5 – API Testing & Integration:** Not Started
* **Phase 6 – Security & Authentication:** Not Started
* **Phase 7 – Docker & CI/CD:** Not Started
* **Phase 8 – Documentation & Final Submission:** Not Started

## Conclusion

The **Smart Campus: Placement Management System** demonstrates the use of microservices and Service-Oriented Architecture to manage campus placement activities efficiently. The system provides separate services for students, companies and jobs, applications, and notifications while supporting secure authentication, role-based authorization, service discovery, and API gateway routing. By providing a centralized platform for students, recruiters, and administrators, the project aims to make the campus placement process more organized, scalable, secure, and efficient.
