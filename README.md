# Prime Medical — Healthcare & Medical Center Management System

![Prime Medical](./PrimeMedical.png)

A comprehensive, full-stack Medical Center Management System built for university semester projects. It provides streamlined healthcare workflows for patients, doctors, nurses, receptionists, pharmacists, and administrators.

---

## 🌟 Key Features

* 🔐 **Role-Based Access Control (RBAC):** Customized dashboards and permissions for Admin, Doctor, Nurse, Receptionist, Pharmacist, and Patient roles.
* 📅 **Appointment Management:** Real-time scheduling, calendar view, and status tracking.
* 🩺 **Medical Consultations & Prescriptions:** Digital consultation notes, vitals recording, and prescription generation.
* 💊 **Pharmacy & Inventory Control:** Stock level alerts, supplier management, and medication dispensing.
* 💳 **Billing & Invoicing:** Automated bill generation, payment tracking, and receipt printing.
* 🤖 **AI Assistant:** Integrated Prime AI Assistant for medical context support and workflow aid.
* 📩 **Multi-Channel Notifications:** Email and SMS notifications for account verification, appointments, and payments.

---

## 🛠️ Technology Stack

* **Backend:** Java 17, Spring Boot 3, Spring Security (JWT), Spring Data JPA, Hibernate, Maven
* **Frontend:** React 18, Vite, Tailwind CSS, Lucide React, Recharts, React Query
* **Database:** MySQL 8.0

---

## 📋 Prerequisites

* **Java:** JDK 17
* **Build Tool:** Maven 3.8+
* **Node.js:** v18+ & npm
* **Database:** MySQL 8.0

---

## 🚀 Local Setup Instructions

### 1. Database Setup

1. Open MySQL CLI or workbench:
   ```sql
   mysql -u root -p
   ```

2. Create the database:
   ```sql
   CREATE DATABASE primemedical_db CHARACTER SET utf8mb4;
   ```

3. Import schema and sample data:
   ```bash
   mysql -u root -p primemedical_db < primemedical_db.sql
   ```

---

### 2. Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. *(Optional)* Set environment variables (PowerShell example):
   ```powershell
   $env:JWT_SECRET = "myVeryLongSecretKey256BitsMinimumForSecurity"
   $env:MAIL_USERNAME = "yourapp@gmail.com"
   $env:MAIL_PASSWORD = "your-gmail-app-password"
   $env:MAIL_FROM = "yourapp@gmail.com"
   ```

3. Run the Spring Boot application:
   ```bash
   mvn spring-boot:run
   ```

   * **Backend API:** `http://localhost:8080`
   * **Swagger UI Documentation:** `http://localhost:8080/swagger-ui.html`

---

### 3. Frontend Setup

1. Open a new terminal and navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies and start the Vite dev server:
   ```bash
   npm install
   npm run dev
   ```

   * **Frontend Web App:** `http://localhost:5173`

---

## 🔑 Test Demo Credentials

All test accounts share the default password: `Password123!`

| Role | Email Address |
| :--- | :--- |
| **Doctor** | `doctor@primemedical.lk` |
| **Nurse** | `nurse@primemedical.lk` |
| **Receptionist** | `reception@primemedical.lk` |
| **Pharmacist** | `pharmacist@primemedical.lk` |
| **Patient** | `patient@primemedical.lk` |
| **Admin** | `admin@primemedical.lk` |

---

## 🧪 Notification Verification Checklist

1. Confirm startup logs display:
   * `Email notifications enabled`
   * `SMS notifications enabled`
2. Register a new user account and verify receipt of confirmation email/SMS.
3. Schedule & cancel an appointment to test channel triggers.
4. Process a payment record to verify billing notifications.

---

## 📜 License

Licensed under the [Apache License 2.0](LICENSE).
