#  Flight Booking Application – Frontend

A **modern, reactive, and role-based Flight Booking frontend application** built using **Angular 17+**, delivering a smooth user experience for flight search, booking, and administration.

---

##  Overview

The **Flight Booking Application (Frontend)** provides a complete interface for users to search and book flights, while offering administrators a powerful dashboard to manage flight inventory.
It is designed with **enterprise-grade architecture**, **JWT-based security**, and **responsive UI principles**.

---

##  Key Highlights

*  Real-time flight search with instant results
*  Secure flight booking & cancellation
*  Admin-only flight management dashboard
*  JWT authentication with role-based access
*  Fully responsive & modern UI
*  Reactive programming using RxJS

---
##  Project Structure

```text
flight-booking-app/
│
├── src/
│   ├── app/
│   │   ├── auth/              # Login & Registration
│   │   ├── user/              # User features
│   │   ├── admin/             # Admin dashboard
│   │   ├── shared/            # Shared services & guards
│   │   ├── core/              # Interceptors & utilities
│   │   └── app.routes.ts
│   │
│   ├── assets/                # Images & animations
│   ├── environments/          # Environment configs
│   ├── styles.scss
│   └── main.ts
│
├── angular.json
├── package.json
└── README.md
```

## Features

###  User Features

* User registration & secure login
* Search flights by source, destination & date
* View detailed flight information
* Book flights with passenger details
* View booking history with PNR
* Cancel bookings with seat restoration
* Profile management & password update
* Secure logout

---

###  Admin Features

* Admin-exclusive dashboard
* Add new flight inventory
* View all flights in a card-based UI
* Monitor active flight statistics
* Real-time seat availability updates
* Smooth animations & loading indicators

---

###  UI / UX Features

* Modern gradient-based UI
* Glass-morphism design elements
* Smooth page transitions
* Reactive form validations
* Custom loading animations
* User-friendly error handling
* Fully responsive layouts
* Animated aircraft & cloud visuals

---

##  Technology Stack

###  Core

* **Angular** 17+ (Standalone Components)
* **TypeScript** 5.x
* **RxJS** 7.x
* **Zone.js**

###  Styling

* **SCSS / Sass**
* **CSS Grid & Flexbox**
* **Angular Animations**

###  API & HTTP

* Angular **HttpClient**
* JWT **HTTP Interceptors**
* Reactive Forms & Validators

###  Routing

* Angular Router
* Route Guards (Auth & Role-based)
* Lazy Loading (where applicable)

---

##  Prerequisites

Ensure the following are installed before running the project:

* Node.js **v18+**
* npm **v9+**
* Angular CLI **v17+**
* Git
* Backend services (Flight & Booking services)
* API Gateway (running and configured)

---

##  Installation

###  Clone the Repository

```bash
cd C:\Users\KIIT\Downloads\chubb_workspace\flightapp-docker\flight-booking-app
```

---

###  Install Dependencies

```bash
npm install
```

---

###  Environment Configuration

Update API Gateway URLs:

**`src/environments/environment.ts`**

```ts
export const environment = {
  production: false,
  apiUrl: 'http://localhost:8080'
};
```

**`src/environments/environment.prod.ts`**

```ts
export const environment = {
  production: true,
  apiUrl: 'https://your-production-api'
};
```

---

###  Run the Application

```bash
npm start
# OR
ng serve
```

 Application runs at:
**[http://localhost:4200](http://localhost:4200)**

---



---

##  Application Architecture

* **Component-Driven Design**
* **Service-based Business Logic**
* **Reactive Data Flow using Observables**
* **JWT Authentication Flow**
* **Role-Based Route Protection**

---

##  Authentication & Authorization

* JWT-based authentication
* Role-based access (USER / ADMIN)
* Route guards to prevent unauthorized access
* Token interceptor for secure API calls

---

## API Integration

* RESTful API communication
* Centralized API services
* Global error handling
* Loading states for async operations

---


---

##  Build & Deployment

### Production Build

```bash
ng build --configuration production
```

Output files will be generated in:

```text
dist/flight-booking-app/
```

---

##  Environment Configuration

Supports:

* Local Development
* Docker Deployment
* Production Builds

Environment files are isolated to ensure **secure & scalable deployment**.

---

