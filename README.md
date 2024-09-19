# Event Manager - Docker Deployment

This repository contains the Docker Compose setup for the Event Manager application, including the backend (Spring Boot), frontend (React), and PostgreSQL database.

## Prerequisites

Before running the application, ensure you have the following installed:

- **Docker**
- **Docker Compose**

## Setup Instructions

### 1. Clone Repositories

First, clone the repositories for both the backend and frontend services:

```
git clone https://github.com/event-manager-cml/event-manager-backend.git
git clone https://github.com/event-manager-cml/event-manager-frontend.git
```

You can also clone this event-manager-deployment repository for the Docker Compose setup:

```
git clone https://github.com/event-manager-cml/event-manager-deployment.git
cd event-manager-deployment
```

### 2. Run with Docker Compose

In the event-manager-deployment directory, use Docker Compose to build and start the services:

```
docker-compose up
```

This command will:

- Pull the latest images for the backend and frontend from Docker Hub.
- Start the backend, frontend, and PostgreSQL database containers.

### 3. Access the Application

Once the containers are running:

- The backend (Spring Boot) will be available at http://localhost:8080
- The frontend (React) will be available at http://localhost:3000

You can interact with the API by visiting the backend’s API endpoint, and the frontend interface by accessing the React application.

### 4. Stopping the Application

To stop the containers, use the following command:

```
docker-compose down
```

This will stop and remove the containers, but the data in the PostgreSQL database will be persisted in a Docker volume.
