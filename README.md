# Ride Booking Platform

📄 **Project Presentation**  
[View Presentation](./Ride-Booking-Platform.pdf)

🎥 **Demo Video**  
[Watch Demo](https://drive.google.com/file/d/1ggLWIXLWlesosH_gK7z9uUth8KW8q0SE/view?usp=sharing)

---

## Overview

Ride Booking Platform is an event-driven microservices application inspired by ride-hailing platforms such as Uber and Ola. The system is designed using Domain-Driven Design (DDD) principles and consists of three core services: Ride Service, Driver Service, and Notification Service.

The platform leverages asynchronous event-driven communication through Kafka/Atropos to manage ride requests, driver matching, trip lifecycle events, payments, and notifications while maintaining scalability, reliability, and loose coupling between services. :contentReference[oaicite:0]{index=0}

---

## Key Features

### Rider Features
- User registration and onboarding
- Fare estimation before booking
- Ride booking and real-time tracking
- Ride cancellation support
- Ride history management
- OTP-based ride start verification
- Email notifications throughout the ride lifecycle

### Driver Features
- Driver registration with vehicle details
- Online/Offline availability management
- Real-time ride offer notifications
- Ride acceptance and assignment workflow
- Assignment cancellation and redispatch handling
- Earnings tracking and settlement
- Email notifications for ride updates

### Platform Features
- Event-driven microservices architecture
- Driver matching and dispatch engine
- Payment lifecycle management
- Notification service integration
- Handling of race conditions and concurrent requests
- Robust ride cancellation and reassignment workflows
- Domain-driven design implementation

---

## Architecture

The platform consists of three independent services:

| Service | Responsibility |
|----------|---------------|
| Ride Service | Ride lifecycle, fare calculation, payments |
| Driver Service | Driver matching, offers, assignments, earnings |
| Notification Service | Rider and driver email notifications |

Services communicate asynchronously through Kafka/Atropos events, ensuring scalability and fault isolation across the platform. :contentReference[oaicite:1]{index=1}

---

## Event-Driven Workflows

The platform supports multiple ride lifecycle scenarios including:

- Ride completion flow
- Rider cancellation before driver assignment
- Rider cancellation after assignment
- Driver cancellation and automatic redispatch
- No-driver-available handling
- Concurrent driver acceptance scenarios
- Ride reassignment workflows
- Payment completion and settlement events

These workflows are implemented using asynchronous event propagation and service orchestration patterns. :contentReference[oaicite:2]{index=2}

---

## Technical Highlights

- Java
- Spring Boot
- PostgreSQL
- Kafka 
- Microservices Architecture
- Domain-Driven Design (DDD)
- Event-Driven Systems
- REST APIs
- Object-Based Access Control
- Email Notification System

---

## Design Artifacts

This repository contains:

- System Architecture Overview
- Sequence Diagrams
- Entity Relationship (ER) Diagrams
- Class Diagrams
- Service Interaction Flows
- Project Presentation
- Demo Video

> Note: This repository contains project documentation and demonstration material only. Source code is not publicly available.

---

## Author

**Mudit Gandhi**