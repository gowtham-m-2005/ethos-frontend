# ETHOS Frontend – React

## System Context

ETHOS is a multi-repository system, where each component is independently deployable but designed to work together as a single ethical decision platform.

This repository contains the frontend user interface for interacting with the ETHOS system.

## Related Repositories

- **ETHOS Backend** – Backend orchestration service for ethical prioritization, persistence, and analytics  
  🔗 https://github.com/gowtham-m-2005/ethos-backend

- **ETHOS Rule Engine** – External ethical evaluation service implemented using rule-based logic  
  🔗 https://github.com/gowtham-m-2005/ethos-python

## Role of This Repository in the System

This frontend acts as the user-facing layer of the ETHOS system, enabling interaction with the backend services through a structured and intuitive interface.

### Responsibilities include:

- Collecting package details from users
- Submitting package data to the backend for ethical evaluation
- Displaying ethically prioritized package lists
- Presenting analytics and system insights
- Supporting administrative monitoring and decision-making

The frontend focuses purely on presentation and interaction, delegating all decision-making and prioritization logic to backend services.

## Application Structure

The frontend is implemented as a single-page application (SPA) using React with client-side routing.

### Key views include:

- **Login Page** – Entry point for system access
- **Package Submission Page** – Interface for submitting new packages for evaluation
- **Admin Dashboard** – View for monitoring prioritized packages and analytics

Routing is handled using React Router, enabling smooth navigation without page reloads.

## System Interaction Flow

1. User submits package details through the frontend interface
2. Frontend sends requests to the backend REST APIs
3. Backend coordinates ethical evaluation and priority assignment
4. Frontend retrieves ranked packages and analytics data
5. Results are rendered dynamically in dashboards and lists

The frontend remains stateless with respect to ethical logic and relies entirely on backend responses.

## Deployment Note

The frontend can be deployed independently as a static web application and communicates with the backend over HTTP. This separation allows independent scaling, UI iteration, and future replacement without impacting backend or rule-engine services.
