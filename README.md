# Hospital Patient Portal - Sprint 2

This repository documents the Sprint 2 MVP for a patient-facing hospital portal. Sprint 2 focused on delivering the core patient journey: secure access, profile completion, doctor browsing, appointment booking through slot hold and confirmation, and appointment viewing.

## Team

- Aayush Ale
- Sanish Ngakhushi
- Mouez Afgan

Scrum Master: Aayush Ale

## Sprint 2 Goal

Deliver a minimum viable product that allows a patient to:

- register and sign in securely
- complete the required profile details
- browse doctors and available appointment slots
- hold and confirm an appointment slot
- view booked appointments and their status

## Sprint 2 Backlog

| No. | User Story | Estimate |
| --- | --- | --- |
| 1 | As a patient, I want to register and sign in securely so that I can access the portal. | 8 story points |
| 2 | As a patient, I want to complete my profile so that I can use the full portal. | 5 story points |
| 3 | As a patient, I want to browse doctors and view available slots so that I can choose a suitable appointment. | 5 story points |
| 4 | As a patient, I want to hold and confirm an appointment slot so that I can complete a booking. | 8 story points |
| 5 | As a patient, I want to view my appointments so that I can track my visits. | 3 story points |

## MVP Delivered In Sprint 2

- Secure patient registration and login
- Patient profile onboarding before full portal use
- Doctor listing and appointment availability browsing
- Appointment slot hold and confirmation flow
- Appointment viewing for the signed-in patient

## Sprint Review

Sprint 2 completed the core MVP patient journey. The main value delivered in this sprint was enabling patients to move from account creation to profile completion, appointment booking, and appointment tracking in one portal flow.

## Technical Overview

This project is structured as a monorepo with a web app and backend services.

### Frontend

- `apps/web` - React, Vite, TypeScript, Tailwind CSS

### Backend Services

- `services/auth-service` - patient authentication and session handling
- `services/patient-service` - patient profile management
- `services/doctor-service` - doctor listing and doctor data
- `services/availability-service` - doctor slot availability
- `services/appointment-service` - appointment hold, confirmation, and appointment queries

### Infrastructure

- PostgreSQL for persistent data
- Redis for temporary slot holds and caching
- Kafka for event-driven communication
- Docker Compose for local orchestration

## Repository Structure

```text
.
├── apps/
│   └── web/
├── services/
│   ├── auth-service/
│   ├── patient-service/
│   ├── doctor-service/
│   ├── availability-service/
│   └── appointment-service/
├── docker-compose.yml
├── Dockerfile.service
├── Dockerfile.web
└── package.json
```

## Repository Note

This README intentionally reflects the Sprint 2 MVP scope from the project report.

Some files in this snapshot reference later-phase or shared modules, including additional services and workspace paths that are not present in this export. In other words, this repository is best read as the Sprint 2 submission snapshot and MVP architecture, rather than a fully cleaned production-ready workspace.

## What Went Well

- The team prioritised the correct MVP features.
- The booking flow delivered the clearest value to patients.
- Profile onboarding helped structure the patient journey before full access.

## Challenges

- Booking work required more coordination than expected because it depended on doctor data, availability, and confirmation logic.
- Lower-priority items were delayed to protect Sprint 2 delivery.

## Future Backlog After Sprint 2

These items were identified for later development after the MVP:

- password recovery and reset
- Google sign-in and OTP fallback
- dashboard summary and quick actions
- appointment cancellation
- medical records management

## Version Control Evidence

Sprint 2 repository reference:

`https://github.com/aayushale001/Software-Engineering-Sprint-2`
