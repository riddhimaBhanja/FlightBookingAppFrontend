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
##  User Account Features Demo


https://github.com/user-attachments/assets/ac14ca69-fe02-418f-bbe2-d8bbde4c441c

---

##  Admin Account Features Demo


https://github.com/user-attachments/assets/dd210f38-28e9-4b92-af24-b6bc1cc9c7ea

---

##  Password Expiration Demo



https://github.com/user-attachments/assets/745728b5-cac1-4a5f-92a8-3c1f1a5f2212



---
##  Overall Flow

![WhatsApp Image 2025-12-23 at 2 15 08 AM](https://github.com/user-attachments/assets/98ab9d5d-0e5b-476c-bfef-1ee89329edab)


---
##  Cancel Booking


![cancel booking](https://github.com/user-attachments/assets/6bb25f7a-b665-4419-9a9b-81f0d1695705)


##  Search Flight


![search_flight](https://github.com/user-attachments/assets/ac02df4a-7634-481d-950a-2d127c46fe32)


![seat selection validation](https://github.com/user-attachments/assets/cf58f72a-9e45-48f8-9828-6051dc07baeb)


##  Seat Booking & its Validation
![seat selection](https://github.com/user-attachments/assets/bb390482-7bdd-4d5a-a4c9-1eecebfebd2f)


##  Validation Errors

##  password expiry validation error

![password_expiry_validation2](https://github.com/user-attachments/assets/ae82164b-3396-4a2f-aede-28f4fea3a407)
![password_expiry_validation](https://github.com/user-attachments/assets/b676bc23-71f4-455d-8055-b771fd79555c)



##  add flight validation error
![add_flight_validation](https://github.com/user-attachments/assets/be39070c-5cb6-4156-828c-bcb9f7e736c4)



##  change password for user validation error


![change_password_validation](https://github.com/user-attachments/assets/02c3fafe-24ad-43dd-9355-63649dad6c98)



##  Booking Flight validation error



![book_flight_validationerror](https://github.com/user-attachments/assets/b4831592-f218-49df-ab54-0dd10bfa3ec2)

---
##  Project Structure

```text
flight-booking-app/
├── src/
│   ├── app/
│   │   ├── components/
│   │   │   ├── home/
│   │   │   ├── login/
│   │   │   ├── register/
│   │   │   ├── search/
│   │   │   ├── inventory/
│   │   │   ├── booking-component/
│   │   │   ├── cancel/
│   │   │   ├── profile/
│   │   │   └── navbar/
│   │   ├── services/
│   │   │   ├── auth.ts
│   │   │   ├── password.ts
│   │   │   └── service.ts
│   │   ├── app.config.ts
│   │   ├── app.html
│   │   ├── app.css
│   │   ├── app.ts
│   │   └── app.route.ts
│   ├── index.html
│   ├── main.ts
│   └── styles.scss
├── angular.json
├── package.json
├── tsconfig.json
└── README.md

```
---


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

