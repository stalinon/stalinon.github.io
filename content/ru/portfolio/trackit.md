---
title: "TrackIt"
image: "trackit_interface.png"
badges:
  - name: "GitHub"
    url: "https://github.com/stalinon/TrackIt"
  - name: "Github Projects"
    url: "https://github.com/users/stalinon/projects/7"

---

**TrackIt** — это веб-приложение для управления личными финансами, включающее в себя учет доходов и расходов, аналитику бюджета, управление лимитами и планируемыми платежами. Также реализована интеграция с Telegram-ботом для уведомлений и взаимодействия с пользователем.  

Приложение реализовано по архитектуре **Clean Architecture** с разделением на слои:  
- **API** (ASP.NET Core Web API)  
- **Application** (CQRS, бизнес-логика)  
- **Domain** (сущности и правила)  
- **Infrastructure** (работа с базой данных и сервисами)  
- **Frontend** (React JS + Redux)  
- **Telegram Bot** (взаимодействие через Telegram API)

---

## Основные возможности
### Веб-интерфейс (React JS + ASP.NET Core API)
- **Регистрация и авторизация** (JWT, Keycloak)
- **Управление финансами**:  
  - Учет доходов и расходов  
  - Категории трат  
  - Лимиты по категориям  
  - Планируемые платежи с напоминаниями  
- **Аналитика**:
  - Отображение баланса  
  - Распределение расходов по категориям  
  - Графики динамики расходов  
- **Подключение Telegram-бота** для получения уведомлений  

### Telegram-бот
- Добавление расходов и доходов через команды  
- Запрос баланса и лимитов  
- Уведомления о планируемых платежах и превышении бюджета  

### Backend API (ASP.NET Core)
- REST API с контроллерами для управления транзакциями, категориями, бюджетом  
- Реализация CQRS (MediatR)  
- Авторизация через JWT и Keycloak  
- Логирование (Serilog) и документация API (Swagger)  

## Технологический стек
**Backend:**
- ASP.NET Core 8.0  
- MediatR (CQRS)  
- Entity Framework Core (PostgreSQL)  
- Serilog (логирование)  
- Keycloak (OAuth2, JWT)  
- Telegram.Bot API  

**Frontend:**
- React TS 
- TypeScript  
- Ant Design 

**Infrastructure:**
- PostgreSQL (хранение данных)  
- Docker (развертывание)  
- Swagger (документация API)  