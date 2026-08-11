# Marketplace Microservices Platform

A production-grade microservices e-commerce platform with asynchronous communication via RabbitMQ.

## Features
- Microservices architecture (Cart, Orders, Inventory, Payments)
- Event-driven design with RabbitMQ
- PayPal checkout integration
- Real-time order tracking
- PostgreSQL with versioned migrations
- API Gateway with Traefik

## Tech Stack
- **Frontend:** React 18 with Vite
- **Backend:** Node.js with Express (4 services)
- **Message Queue:** RabbitMQ (topic exchange)
- **Database:** PostgreSQL
- **API Gateway:** Traefik
- **DevOps:** Docker Compose

## Getting Started

### Prerequisites
- Node.js v16+
- PostgreSQL 13+
- RabbitMQ 3.8+
- Docker (optional)

### Installation

```bash
# Frontend
cd frontend
npm install
npm run dev

# Services (each runs independently)
cd services/cart
npm install
npm start

cd services/orders
npm install
npm start

cd services/inventory
npm install
npm start

cd services/payments
npm install
npm start
```

### With Docker
```bash
docker-compose up
```

## Architecture
- Independent microservices for Cart, Orders, Inventory, Payments
- Asynchronous communication via RabbitMQ events
- Service-per-database pattern
- Event-driven order flow

## Learning Outcomes
- Microservices architecture and design
- Asynchronous messaging with RabbitMQ
- Distributed systems patterns (Saga, Event Sourcing)
- API Gateway patterns
- Independent service scalability
- Payment integration (PayPal)

## Author
Omar Adel Mohamed
- GitHub: [@omaradel](https://github.com/omaradel)
- Email: omarabousaif1413@gmail.com

## License
MIT License