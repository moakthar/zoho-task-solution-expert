# 🚲 Multi-Floor Cycle Parking System - High Level Design (HLD)

## 📘 Overview
This project expands the cycle parking system into a **10-floor smart parking building**.  
Each floor has dimensions **560 × 20 units**, with one floor designated as a **Security Floor** (reduced slots, surveillance office, and monitoring staff).

The system integrates **IoT devices, cloud backend services, and user applications** to provide:
- Real-time slot availability
- Smart booking and reservations
- Theft tracking and insurance
- Role-based access for users, staff, and administrators

---

## 🏗️ System Components

### Physical Layout
- **6-row parking zones** per floor, with defined crossings and pathways.  
- **Entry/Exit gates** equipped with QR, RFID, and license plate recognition.  
- **Sensors and smart locks** at each slot for occupancy detection.  
- **CCTV cameras** for surveillance and theft monitoring.  
- **Security floor** with surveillance room and reduced parking capacity.  

### Application Features
- **User/Admin portal** to check availability and manage reservations.  
- **On-the-fly updates** from sensors to backend.  
- **Notifications** for full parking, booking confirmations, and alerts.  

---

## 🔧 Technical Architecture

### Frontend
- Built using **React** or **Angular**.  
- Features: Booking interface, real-time slot map, dashboards, notifications.  
- *Note:* Not required in prototype.  

### Backend
- Implemented with **Node.js (Express/NestJS)** or **Java (Spring Boot)**.  
- Core Services:  
  - Reservation Service  
  - Theft Tracking Service  
  - Insurance Service  
  - Notification Service  
  - API Gateway  

### Databases
- **PostgreSQL (Julius)** – structured relational data.  
- **MongoDB** – unstructured KYC, CCTV logs.  
- **Kafka** – event streaming (slot updates, notifications, audit logs).  

### Identity & KYC
- **3rd-party providers**: Onfido, IDfy, Socure.  
- **Authentication**: Keycloak / Auth0 / custom OIDC.  
- Role-based access (User, Security Staff, Admin).  

### Monitoring & Logging
- **Prometheus + Grafana** for metrics & dashboards.  
- **ELK Stack** for log aggregation and analysis.  

### Edge/IoT Layer
- Smart locks and sensors managed via **floor controllers**.  
- CCTV feeds processed locally and streamed securely.  
- IoT Gateway with encrypted communication to backend.  

---

## 📊 Diagrams
- **HLD Diagram** (system layers and components).  
- **Parking Layout Diagram** (6-row design, entry/exit, pathways).  
- **UML Class Diagram** (Cycle, ParkingRow, User, Sensor, Notification).  
- **UML Sequence Diagram** (slot request → assignment → confirmation).  

*(All diagrams available in `.puml` or `.drawio` format in the `/diagrams` folder)*  

---

## 🚀 Features
- Multi-floor parking management (10 levels).  
- Smart reservations with **real-time updates**.  
- Security floor for surveillance & monitoring.  
- Integrated theft tracking and insurance management.  
- Notifications for booking, slot availability, and incidents.  

---

## 📂 Project Structure
