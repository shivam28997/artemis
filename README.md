# Apache ActiveMQ Artemis - Dockerized Broker

This project sets up an Apache ActiveMQ Artemis message broker using Docker Compose. It includes a persistent data volume and a custom broker configuration.

## Features

- Custom authentication (admin:admin)
- Durable queue setup (test-queue)
- Persistent message storage
- Custom broker configuration via broker.xml
- Web Console access at http://localhost:8261
- JMS port mapped to 62626

## Prerequisites

- Docker
- Docker Compose

## Folder Structure

.
├── docker-compose.yml              # Docker setup for Artemis broker  
├── artemis-data/                   # Persistent volume for message data  
└── broker-config/  
    └── broker.xml                  # Custom broker configuration file

## How to Use

### 1. Start the Broker

```bash
docker-compose up -d
