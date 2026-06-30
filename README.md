# Project Atlas (Atlas POS) 🚀

Project Atlas is a modern, enterprise-grade, cloud-based Point of Sale (POS) and Fiscal Management solution tailored for retail and commercial business environments. 

This repository showcases a full-stack implementation utilizing a high-performance **.NET Web API Backend** paired with a highly reactive, optimized **Angular Frontend**.

---

## 🛠️ Tech Stack & Architecture

### Frontend (Angular)
*   **Angular 19+ / 20+:** Built entirely using modern **Standalone Components** (moving away from legacy NgModules).
*   **State Management:** Powered by **Angular Signals** (`signal`, `computed`, and `effect`) to deliver a blazing-fast, grain-level reactive UI.
*   **Control Flow:** Implemented the modern syntax (`@if`, `@for`, `@switch`) for cleaner template logic and improved rendering performance.
*   **Performance Optimization:** Leveraging **Deferrable Views (`@defer`)** to lazy-load heavy UI elements, graphs, and complex tables on demand.
*   **Forms Management:** Built with complex, dynamic **Reactive Forms** using `FormArray` for real-time item invoice generation and instant client-side calculations.

### Backend (.NET)
*   **Core Engine:** .NET Core Web API leveraging C# and top-tier enterprise standards.
*   **Architecture:** Strictly follows **Clean Architecture (Domain-Driven Design principles)** separating Domain, Application, Infrastructure, and WebAPI layers.
*   **Patterns:** Implemented **CQRS (Command Query Responsibility Segregation)** via **MediatR** to ensure decoupled, highly scalable, and maintainable business logic.
*   **Data Access:** Entity Framework Core utilizing a code-first approach with optimized LINQ queries, indexation, and repository patterns.

---

## 💡 Key Features Covered

1.  **Dynamic Invoicing Module:** Real-time calculation of totals, taxes, and discounts as items are dynamically added or modified.
2.  **Role-Based Security:** End-to-end authentication and authorization using secure **JWT (JSON Web Tokens)** with custom route guards in Angular.
3.  **Real-Time Dashboard:** Interactive sales data visualization using modern charting libraries, optimized with Angular lifecycle hooks.
4.  **Resilient HTTP Interceptors:** Global interceptor implementation for automatic token injection and structured, user-friendly API error handling.

---

## 🚀 How to Run Locally

### Prerequisites
*   .NET SDK (Latest version)
*   Node.js (LTS version) & Angular CLI
*   SQL Server (or Docker instance)

### Backend Setup
1. Clone the repository: `git clone https://github.com/gabriel9107/atlas-pos-core.git`
2. Navigate to the API folder: `cd backend/Atlas.WebApi`
3. Update the connection string in `appsettings.json`.
4. Run migrations: `dotnet ef database update`
5. Start the server: `dotnet run`

### Frontend Setup
1. Navigate to the client folder: `cd frontend`
2. Install dependencies: `npm install`
3. Run the development server: `ng serve -o`
