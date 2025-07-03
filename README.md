# Insurance-Management-System

## Description
 
IMS is a robust and secure Insurance Management System built with .NET Core Web API and SQL Server. It manages core modules like Users, Customers, Agents, Policies, Claims, and Notifications, and implements **JWT-based role-based authentication** for Admin, Customer, and Agent users.
 
## Technologies Used
 
- Backend: ASP.NET Core Web API
- Database: SQL Server (SSMS)
- Architecture: Clean Architecture (Controller, Services, Repositories, DTOs)
- Authentication: JWT Token with Role-based Authorization
- Object Mapping: AutoMapper
- Testing: xUnit (if applicable)
- Documentation: Swagger UI
- Logging: Serilog
- Frontend: (If applicable, like Angular/React, mention here)
 
## Project Structure
 
**src/**
├── index.html
├── main.ts
├── styles.css
├── test.ts
├── app/
│   ├── app.component.html
│   ├── app.component.css
│   ├── app.component.spec.ts
│   ├── app.component.ts
│   ├── app.config.ts
│   ├── app.routes.ts
│   ├── core/
│   │   ├── auth/
│   │   │   ├── auth.services.ts
│   │   │   ├── auth.guards.ts
│   │   ├── intercepter/
│   │   ├── services/
│   ├── features/
│   │   ├── admin/
│   │   │   ├── admin-dashboard/
│   │   │   ├── admin-profile/
│   │   │   ├── agent-management/
│   │   │   ├── customer-management/
│   │   │   ├── policy-management/
│   │   ├── agent/
│   │   ├── auth/
│   │   │   ├── login/
│   │   │   ├── register/
│   │   ├── customer/
│   │   ├── Home/
│   │   ├── products/
│   ├── layouts/
│   │   ├── admin-layout/
│   │   ├── agent-layout/
│   │   ├── customer-layout/
│   ├── shared/
│   │   ├── components/
│   │   ├── confirm-dialog/
│   │   ├── reject-dialog/
│   │   ├── api-response.interface.ts
│   │   ├── pagedResult.dto.ts
├── environment/
│   ├── environment.development.ts

 
## User Roles & Permissions
 
- **Admin:** Manage all modules
- **Agent:** Handle policies and claims
- **Customer:** Request/view policies, submit claims
 
## Authentication
 
- Implemented JWT-based login with 3 roles
- Secured endpoints with `[Authorize(Roles = "Admin")]`, etc.
 
## Features Implemented
 
- ✅ User Registration & Login (JWT Auth)
- ✅ CRUD for Customers, Agents, Policies, Claims
- ✅ Role-based access
- ✅ Logging with Serilog
- ✅ Exception handling middleware
- ✅ Swagger integrated
- ✅ Clean Architecture using Interfaces, Repositories, Services
- ✅ AutoMapper configured
- ✅ SQL Server DB-first approach with Scaffolded Models
 
## API Testing
 
- Use Swagger or Postman to test endpoints
- Include Authorization Header with Bearer Token
 
## Setup Instructions

Add your connection string in appsettings.json.
Run the project:
dotnet run

For installation:
npm i

Run the Project :
ng serve

