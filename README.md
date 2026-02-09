🏛️ University Management Web API
A robust, multi-layered Web API built with ASP.NET Core 8 to manage university operations. This project implements a decoupled architecture to ensure scalability, maintainability, and clear separation of concerns.

🏗️ Architecture & Project Structure
The solution is divided into three main layers to follow industry best practices:

🌐 University.Api: The presentation layer containing Controllers and Swagger configurations for frontend interaction.

🧠 University.Core: The business logic layer where Services, DTOs (Data Transfer Objects), and Validations reside.

💾 University.Data: The data access layer handling SQL Server connections via Entity Framework Core, including Migrations, Entities, and Repositories.

🚀 Key Features
RESTful API Design: Clean and intuitive endpoints for managing students, courses, and instructors.

Swagger/OpenAPI Integration: Interactive API documentation for easy testing and frontend integration.

Repository Pattern: Abstracted data access logic for better testability.

DTO Mapping: Secure data transfer between layers to hide sensitive entity details.

Fluent Validation: Robust input validation to ensure data integrity.

🛠️ Tech Stack
Backend: .NET 8 Web API

ORM: Entity Framework Core (Code First)

Database: Microsoft SQL Server

Documentation: Swagger UI

Patterns: Dependency Injection, Repository Pattern, Unit of Work.

📂 Layer Details
1. Data Layer (University.Data)
Contexts: Database context for EF Core.

Entities: Database table models.

Migrations: Database version control.

2. Core Layer (University.Core)
Services: Concrete business logic implementations.

Validations: Logic to verify incoming data.

Exceptions: Custom error handling for the domain.

3. API Layer (University.Api)
Controllers: Handling HTTP requests.

Filters: Global exception handling and logging.
