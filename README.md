# ECommerce API

![.NET](https://img.shields.io/badge/.NET-9.0-blueviolet)
![build](https://img.shields.io/badge/build-passing-brightgreen)

A modern .NET 9 Web API for e-commerce scenarios, organized with Onion Architecture to keep domain rules at the center and infrastructure concerns on the outside.

---

## Purpose

- Provide a reference backend covering catalog, basket, order, and payment journeys.
- Highlight how Onion Architecture separates core domain logic from application and infrastructure layers.
- Offer a solid foundation for teams extending commerce or marketplace capabilities.

---

## Project Structure

ECommerce.sln
├── Core
│ ├── ECommerce.Domain
│ ├── ECommerce.Abstraction
│ └── ECommerce.Service
├── Infrastructure
│ ├── Persistence
│ └── Presentation
├── ECommerce.Web
└── Shared


---

## 🔑 Main Features

- JWT authentication for secure access control.
- Product catalog filtering, sorting, and pagination for better discovery.
- Redis-backed shopping basket for fast, resilient cart experiences.
- Order and payment pipeline for reliable checkout flows.
- Global exception handling for consistent error responses.
- Swagger/OpenAPI documentation for easy API exploration.

---

## 🧱 Architecture Overview

- **Core:** Pure domain concerns — entities, contracts, and specifications with no outward dependencies.
- **Infrastructure:** Implements persistence, repositories, seeding, Redis, and external integrations.
- **Web:** Hosts the ASP.NET Core pipeline, controllers, middleware, and Swagger UI.
- **Shared:** Provides DTOs, pagination helpers, and reusable error models for all layers.

---

## 🚀 Getting Started

1. Restore dependencies:

   ```bash
   dotnet restore
Apply migrations in Infrastructure Layer.

Run the API:

dotnet run --project ECommerce/ECommerce.Web.csproj


Open Swagger UI to explore endpoints:

https://localhost:7286/swagger
🤝 Contributing

Contributions are welcome.
Please discuss major proposals via issues before submitting pull requests.
