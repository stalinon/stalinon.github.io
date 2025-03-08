---
title: "TrackIt"
image: "trackit_interface.png"
badges:
  - name: "GitHub"
    url: "https://github.com/stalinon/TrackIt"
  - name: "Github Projects"
    url: "https://github.com/users/stalinon/projects/7"

---

**TrackIt** is a web application for personal finance management, including income and expense tracking, budget analysis, category limits management, and scheduled payments. It also features integration with a Telegram bot for notifications and user interaction.  

The application follows **Clean Architecture** with a layered structure:  
- **API** (ASP.NET Core Web API)  
- **Application** (CQRS, business logic)  
- **Domain** (entities and rules)  
- **Infrastructure** (database operations and services)  
- **Frontend** (React JS + Redux)  
- **Telegram Bot** (interaction via Telegram API)  

---

## Key Features
### Web Interface (React JS + ASP.NET Core API)
- **Registration and Authentication** (JWT, Keycloak)
- **Finance Management**:  
  - Tracking income and expenses  
  - Expense categories  
  - Setting spending limits  
  - Scheduled payments with reminders  
- **Analytics**:
  - Displaying balance  
  - Expense distribution by category  
  - Spending trends charts  
- **Telegram Bot Integration** for notifications  

### Telegram Bot
- Adding expenses and income via commands  
- Checking balance and spending limits  
- Notifications for scheduled payments and budget overages  

### Backend API (ASP.NET Core)
- REST API with controllers for transactions, categories, and budgeting  
- CQRS implementation (MediatR)  
- Authentication via JWT and Keycloak  
- Logging (Serilog) and API documentation (Swagger)  

## Technology Stack
**Backend:**
- ASP.NET Core 8.0  
- MediatR (CQRS)  
- Entity Framework Core (PostgreSQL)  
- Serilog (logging)  
- Keycloak (OAuth2, JWT)  
- Telegram.Bot API  

**Frontend:**
- React TS  
- TypeScript  
- Ant Design  

**Infrastructure:**
- PostgreSQL (data storage)  
- Docker (deployment)  
- Swagger (API documentation)  
