# Microservices-Task

# Forked the given repo https://github.com/mohanDevOps-arch/Microservices-Task.git

<img width="898" height="187" alt="image" src="https://github.com/user-attachments/assets/834df340-3253-4226-ade0-1ee3c67180d9" />


## Overview
This document provides details on testing various services after running the `docker-compose` file. These services include User, Product, Order, and Gateway Services. Each service has its own endpoints for testing purposes.

#Services Overview

The application consists of three independent microservices:

Service	Port	Description
User Service	3000	
Product Service	3001	
Gateway Service	3000
Order Service 3002

## Dockerfile

Each service contains a Dockerfile with the following configuration:

Uses official Node.js base image
Sets working directory
Copies project files
Installs dependencies using npm install
Exposes service-specific port
Runs application using CMD

<img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/0273fca4-68d5-49da-93fc-d282fc9a1b04" />

<img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/0dd962e1-8b29-4bc5-9ca0-7d2ad8f7eda3" />

<img width="940" height="527" alt="image" src="https://github.com/user-attachments/assets/398b8f2f-3136-43b1-b6d7-7e176a4ec3fe" />

<img width="940" height="530" alt="image" src="https://github.com/user-attachments/assets/9b383202-f0ae-4252-bc38-1fc3197a431e" />

## Docker Compose Configuration

The docker-compose.yml file:

Defines all three services
Maps ports:
3000 → User Service
3001 → Product Service
3003 → Gateway Service
Creates a shared network for inter-service communication

<img width="940" height="528" alt="image" src="https://github.com/user-attachments/assets/49ca6972-c021-4f58-88b4-7a8fb6d44d1e" />

## Had an issue while running the docker-compose. Please find the error below. npm error.

<img width="1723" height="719" alt="image" src="https://github.com/user-attachments/assets/088422a2-277c-4a40-993f-c6f8e116fee7" />

Resolved it by adding start service in all the services json package.


# Docker compose 

docker-compose up --build 

<img width="1918" height="994" alt="image" src="https://github.com/user-attachments/assets/8e3d5e73-2e79-4a71-bd28-df459eece637" />

<img width="1915" height="1029" alt="image" src="https://github.com/user-attachments/assets/d2173c39-4846-4abf-84ec-976315ac071e" />






