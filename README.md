---# DVLD

# 🚗 Driving & Vehicle License Department (DVLD) System

An end-to-end management system designed to streamline and automate procedures for issuing and managing driving licenses, applications, test appointments, user permissions, and license detentions.

Built using **C#** and designed following a clean **N-Tier Architecture** to strictly separate data access, business logic, and presentation layers.

---

## 📌 Key Features

* **Application Management:**
  * First-time driving license issuance.
  * Driving license renewal.
  * Replacement for lost or damaged licenses.
  * International driving license issuance (for Class 3 license holders).
  * Release of detained licenses upon fine settlement.

* **Test Workflow & Business Rules:**
  * Sequential 3-stage test process: **Vision Test** $\rightarrow$ **Written Test** $\rightarrow$ **Street Test**.
  * Age eligibility and duplicate application validation per license class.
  * Retest tracking and fee calculations.

* **System & Security Administration:**
  * **User Management:** Create, update, deactivate accounts, and manage permissions.
  * **People Management:** Centralized registry queried by National ID to eliminate duplicates.
  * **License Detention:** Detain licenses with custom fines/reasons and release them.
  * **Audit Logging:** System-wide tracking of user actions and timestamps.

---

## 🛠️ Tech Stack & Architecture

* **Programming Language:** C# (.NET Framework / Windows Forms)
* **Database:** Microsoft SQL Server (ADO.NET)
* **Architecture:** N-Tier Architecture
  * `DVLD_BusinessAccess` (Business Logic Layer)
  * `DVLD_DataAccess` (Data Access Layer)
  * `DVLD_Presentation` (UI Layer)

---

## 📊 Driving License Classes

| Class | Name | Minimum Age | Fees | Validity |
| :--- | :--- | :---: | :---: | :---: |
| **Class 1** | Small Motorcycle | 18 | $15 | 5 Years |
| **Class 2** | Heavy Motorcycle | 21 | $30 | 5 Years |
| **Class 3** | Ordinary Driving License (Car) | 18 | $20 | 10 Years |
| **Class 4** | Commercial (Taxi/Limousine) | 21 | $200 | 10 Years |
| **Class 5** | Agricultural Vehicles | 21 | $50 | 10 Years |
| **Class 6** | Small & Medium Buses | 21 | $250 | 10 Years |
| **Class 7** | Heavy Vehicles & Trucks | 21 | $300 | 10 Years |

