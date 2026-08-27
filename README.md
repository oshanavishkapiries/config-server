# ⚙️ Spring Cloud Config Server

**Module**: Enterprise Cloud Architecture (ITS 2130)  
**Component**: Microservices Platform Infrastructure

---

## 👤 Student Information (Section 12 Compliance)

- **Student Name**: OSHAN AVISHKA
- **Student Number**: 241711058
- **Slack Handle**: @oshanavishka
- **GCP Project ID**: itc-2130-eca

---

## 📖 Component Description

`config-server` is a centralized configuration management server built with **Spring Cloud Config Server**. It externalizes and centralizes configuration properties across all microservices (Book Service, User Service, Order Service, API Gateway, Eureka Server) in the cluster.

### Key Features
- Centralized externalized configuration management.
- Dynamic environment configuration switching.
- High-availability deployment support across multi-zone GCP Compute Instances.

---

## 🛠️ Technology Stack

- **Framework**: Java 21 / Spring Boot 3.3.3
- **Spring Cloud**: Spring Cloud Config Server (2023.0.3)
- **Port**: `8888`
- **Process Management**: PM2 (Non-containerized VM deployment)

---

## 🚀 Setup & Getting Started Instructions

### Build & Run locally
```bash
# Build JAR file
mvn clean package -DskipTests

# Run using Java
java -jar target/config-server-1.0.0.jar
```

### Run using PM2 (GCP VM / Production)
```bash
pm2 start target/config-server-1.0.0.jar --name config-server
```

---

## 🔗 Repository Navigation & Structure

This repository is maintained as a Git Submodule inside the parent super-repository:
- 🏛️ **Parent Repository**: [eca-microservices-platform](https://github.com/oshanavishkapiries/eca-microservices-platform)
