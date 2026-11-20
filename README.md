# 🏥 MediCore | Hospital Management System

## 📖 Project Description

**MediCore** is a comprehensive, full-stack hospital workflow and healthcare administration web platform
engineered using **Node.js**, **Express.js**, and **MySQL**. Designed to modernize hospital operations and replace fragmented, paper-based record-keeping, MediCore brings together clinical, administrative, and operational workflows into a single unified digital system.

At the core of the platform is a carefully normalized **relational database schema** that manages centralized records across multiple hospital modules—including patient demographics, Outpatient Department (OPD) consultations, doctor and nursing staff rosters, inpatient room allocations, patient billing, and pharmaceutical inventory. 
Rather than relying solely on application-level logic, MediCore leverages **automated MySQL database triggers** to enforce data integrity and automate routine administrative tasks at the database layer.
These triggers dynamically assign nursing shifts, automatically archive departing employee records for audit compliance, manage department head transitions, and update real-time room availability as patients are admitted or discharged .

On the backend, the system exposes clean, modular **RESTful API endpoints** paired with **role-based access workflows** to ensure secure data persistence, fast query execution, and reliable communication between hospital departments. 
The frontend is built with **HTML5, CSS3, and Vanilla JavaScript** as a responsive, single-page interface that allows hospital administrators and staff to perform real-time lookups, register patients, manage staff schedules, and monitor ward occupancy seamlessly from any browser. 
Deployed in the cloud using **Render** and **Aiven Managed MySQL**, MediCore demonstrates end-to-end production architecture from database modeling to live web hosting.

---

## ✨ Key Features

* **Centralized Patient & OPD Management:** Register patients, track outpatient consultations, and maintain persistent medical histories.
* **Automated MySQL Database Triggers:** Built-in database triggers handle dynamic nurse shift assignments, employee record archiving, department head updates, and real-time room occupancy tracking.
* **Clinical Staff & Employee Administration:** Manage doctors, nurses, and administrative staff schedules and department mappings.
* **Billing & Pharmaceutical Tracking:** Streamlined management of patient billing and pharmacy stock records.
* **RESTful API & Role-Based Workflows:** Structured backend API endpoints ensuring secure data persistence and smooth operational workflows.

---

## 🛠️ Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MySQL (Relational Schemas & Automated Database Triggers)
* **Frontend:** HTML5, CSS3, Vanilla JavaScript
* **Deployment & Cloud:** Render (Web Service), Aiven (Managed Cloud MySQL)

---

## 📂 Project Structure

```text
Hospital-Management-System/
├── routes/
│   ├── patients.js       # Patient & OPD REST API endpoints
│   ├── employees.js      # Clinical staff & shift management endpoints
│   └── general.js        # Rooms, billing, pharmacy & general endpoints
├── db.js                 # MySQL connection pool configuration (with SSL support)
├── server.js             # Express server & static frontend hosting
├── index.html            # Single-page responsive frontend interface
├── schema.sql            # Relational database schema, tables & MySQL triggers
├── package.json          # Project dependencies & scripts
└── .gitignore            # Environment & dependency exclusions

```

**Live Demo:** [https://hospital-management-system-hzaq.onrender.com/](https://hospital-management-system-hzaq.onrender.com/)
