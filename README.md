# Pet Clinic - Frontend Web Application

A simple web interface that consumes the Pet Clinic backend microservices (owner-service, pet-service, appointment-service) through the API Gateway.

## Student Information
- **Student Name:** Isuri Gamage
- **Student Number:** 241722008
- **Slack Handle:** 
- **GCP Project ID:** 

## Live Deployment
🔗 **Deployed URL:** 

## Project Description
This is the frontend application for the Pet Clinic Management System. It provides a functional interface for managing pet owners, pets, and veterinary appointments. All requests are sent through the API Gateway, which routes them to the appropriate backend microservice using service discovery. The frontend demonstrates that all three backend microservices are accessible and functioning correctly, fulfilling the module's frontend requirement.

## Technology Stack
- **Frontend:** Plain HTML5, CSS3, JavaScript (Fetch API)
- **Backend Communication:** REST API calls through the API Gateway
- **Cloud Platform:** Google Cloud Platform (GCP) — deployed as PaaS/Serverless on Cloud Run

## Features
- Create, view, update, and delete pet owners
- Create, view, update, and delete pets
- Book, view, update, and delete veterinary appointments
- All operations routed through the API Gateway (`/api/owners`, `/api/pets`, `/api/appointments`)

## Setup / Getting Started

### Prerequisites
- The Pet Clinic backend system must be running (eureka-server, config-server, api-gateway, owner-service, pet-service, appointment-service)
- A modern web browser

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/Isuri15/frontend-web-app.git
   cd frontend-web-app
   ```
2. Open `index.html` in a browser using a local web server (recommended, to avoid CORS/`file://` issues), for example with VS Code's Live Server extension, or:
   ```bash
   python3 -m http.server 5500
   ```
3. Navigate to `http://localhost:5500/index.html`.
4. In the "API Gateway Base URL" field, enter the address of the running API Gateway (e.g. `http://localhost:8080` for local testing, or the Cloud Load Balancer URL when deployed).

## Cloud Deployment
This frontend is deployed on Google Cloud Platform using **Cloud Run** (PaaS/Serverless model), as required by the module's cloud deployment guidelines. It communicates with the backend microservices platform, which is deployed separately using an IaaS model on Compute Engine.

## Related Repositories
- [backend-microservices-platform](https://github.com/Isuri15/backend-microservices-platform)
- [backend-services](https://github.com/Isuri15/backend-services)
