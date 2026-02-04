# 🏥 Patient Management System  
**Microservices Architecture | Spring Boot | AWS | LocalStack | gRPC**

A **cloud-native, microservices-based Patient Management System** built using **Spring Boot**, **API Gateway**, **gRPC**, and **AWS services**, with **LocalStack** for local cloud simulation.

This project demonstrates **enterprise-grade backend engineering**, **service-to-service communication**, and **infrastructure-as-code**, aligned with real-world healthcare platforms.

---

## 🚀 Key Features

- 🧩 Microservices-based architecture
- 🌐 Centralized API Gateway
- 🔐 Authentication & Authorization Service
- 🏥 Patient Management Service
- 💳 Billing Service with gRPC communication
- 📊 Analytics Service
- ☁️ AWS services simulated using LocalStack
- 📦 Infrastructure as Code (CloudFormation)
- 🧪 Integration testing support

---

## 🏗️ System Architecture

```text

Client
  ↓
API Gateway
  ↓
---------------------------------
| Auth Service                  |
| Patient Service               |
| Billing Service (gRPC)        |
| Analytics Service             |
---------------------------------
  ↓
AWS Services (LocalStack)
- RDS (PostgreSQL)
- S3
- ELB
```

# 📂 Repository Structure

```text

patient-management/
├── api-gateway/                 # Central API Gateway
├── auth-service/                # Authentication & authorization service
├── patient-service/             # Patient domain & medical records
├── billing-service/             # Billing & payments (gRPC-based)
├── analytics-service/           # Reporting & analytics
├── grpc-requests/
│   └── billing-service/         # gRPC proto definitions
├── api-request/                 # API request samples
├── integration-test/            # End-to-end integration tests
├── infrastructure/              # AWS + LocalStack + CloudFormation
├── .gitignore
└── README.md
````

# 🛠️ Tech Stack

## Backend
- Java 17
- Spring Boot
- Spring Cloud
- Spring Data JPA
- Hibernate

## Communication
- REST APIs
- gRPC (inter-service communication)

## Database
- PostgreSQL
- AWS RDS (simulated via LocalStack)

## Cloud & DevOps
- AWS (RDS, S3, ELB)
- LocalStack
- AWS CloudFormation
- Docker & Docker Compose

## Tools
- Maven
- Postman
- Git & GitHub

# 🔗 Core Services

## 🌐 API Gateway
- Central entry point for all client requests
- Routes requests to appropriate microservices
- Abstracts internal service architecture

## 🔐 Auth Service
- Authentication and authorization
- Token-based security (JWT-ready)

## 🏥 Patient Service
- Patient registration and profile management
- Medical records handling

## 💳 Billing Service
- Billing and payment processing
- gRPC-based internal service communication

## 📊 Analytics Service
- Generates reports and analytics
- Provides insights into patient and billing data

# ⚙️ Run Locally (AWS via LocalStack)

## Prerequisites
- Java 17+
- Maven
- Docker & Docker Compose
- AWS CLI

---

## 1️⃣ Start LocalStack & Infrastructure

```bash
docker compose up -d
