# Multi-Level Car Parking System

## Overview
This project provides a **High-Level Design (HLD)** and architecture for a **multi-level car parking facility**.  
It covers both the **physical facility blueprint** and the **software system architecture** to enable smart, secure, and efficient parking management.

---

## Facility Blueprint
The car parking facility is designed with:
- **Ground Floor**
  - Main Entry & Exit
  - Ramp Access
  - Reception & Elevator Lobby
  - Stairwell Access
- **Typical Parking Floors**
  - Standard Slots, Accessible Slots, EV Charging Slots
  - Vehicle Ramp Up/Down
  - Pedestrian Stairwell & Elevator Access
- **Roof Top Parking**
  - Open Air Parking
  - EV Charging Area
- **Facility Management**
  - Control Room
  - Maintenance
  - Security Office

---

## System Architecture
The smart parking system includes multiple layers:

1. **Physical Layer**
   - Parking Structure, Gates, Elevators, CCTV, Sensors
2. **Network & Device Layer**
   - IoT Sensors, Smart Kiosks, Cameras, Network Infrastructure
3. **Application Layer**
   - Slot Allocation Service  
   - Vehicle Auth Service  
   - Billing & Payments Service  
   - Notification Service  
   - Analytics Service
4. **Data Layer**
   - SQL/NoSQL Databases  
   - Event Streaming (Kafka)
5. **Security & Compliance**
   - IAM, Encryption, Logging, RBAC
6. **Integration Layer**
   - APIs, Mobile Apps, Kiosks, Dashboards, Payment Gateways, Law Enforcement

---

## Features
- Real-time slot allocation and monitoring
- Vehicle authentication via RFID/ANPR
- EV charging and billing
- CCTV surveillance
- Admin dashboards & mobile apps
- Scalable microservices with Kubernetes deployment

---

## How to Use
- **Diagrams**: Open the `.drawio` or `.puml` files in `/diagrams`
- **Code Samples**: Available in `/samples`
- **Docs**: See `/hld` for full High-Level Design document

---

## References
- Parking lot design standards — ITE Parking Guide  
- Microservices architecture best practices — CNCF  
- IoT sensor integration — vendor documentation
