# 🚀 Acme EMS — Enterprise Employee Management System

> **Live Application:** [https://acme-ems.web.app/](https://acme-ems.web.app/)

---

## 📖 Project Overview

**Acme EMS** is a comprehensive, cloud-native Employee Management System designed to handle the complex organizational hierarchy, attendance, field-sales tracking, and HR operations of a modern enterprise. 

Built entirely as a secure, high-performance web application, it provides a centralized dashboard for administrators, localized views for departmental managers, and a streamlined mobile-friendly interface for field agents and general staff. 

## 🛠️ Technical Stack & Architecture

Engineered for speed, offline-capability, and zero-maintenance scaling using a modern serverless approach.

- **Frontend UI:** Vanilla JavaScript (ES6+), HTML5, CSS3 (Custom responsive design system using CSS Variables, zero heavy frameworks for sub-second load times).
- **Cross-Platform Mobile:** **Capacitor.js** integration to compile the web application into a native **Android** application (`.apk`/`.aab`), providing native device features and a true app-like experience for field agents.
- **Backend & Database:** Firebase Serverless Architecture & Cloud Firestore (NoSQL).
- **Authentication:** Firebase Auth with hardened security rules and lockout mechanics.
- **Geolocation & Mapping:** Leaflet.js integrated with native browser and device Geolocation APIs.
- **Data Processing:** SheetJS for high-performance, client-side Excel `.xlsx` parsing and generation.
- **Data Visualization:** Chart.js for responsive, canvas-based analytics.

## ✨ Core Features & Capabilities

### 📱 Cross-Platform Deployment (Web & Android)
A unified codebase that runs seamlessly in modern desktop browsers and compiles into a native Android app via **Capacitor**. Field agents get a responsive native experience with native splash screens, while managers access the expansive web dashboard from their PCs.

### 🛡️ 6-Tier Role-Based Access Control (RBAC)
A robust hierarchical security model ensuring users only access data appropriate for their organizational level.
- **L1 & L2 (Staff / Sr. Staff):** Self-service attendance, task viewing, and leave requests.
- **L3 & L4 (Supervisors / Regional Managers):** Team attendance, initial leave approvals, task assignment, and field tracking for direct reports.
- **L5 (Head of Department):** Department-wide analytics, final leave approvals, and secure data exports (financials redacted).
- **L6 (Admin / Director):** Full administrative access. Global organizational view, raw data imports/exports, user management, and system configuration.

### 📍 Real-Time Sales & Field Tracking
Built for modern distributed teams and field agents.
- **Live Location Pings:** Background GPS tracking records agent coordinates, rendered dynamically via **Leaflet.js** on manager dashboards.
- **Field Visit Logs:** Sales reps can log client meetings with integrated map coordinates, lead temperature (Hot/Warm/Cold), pricing quotes, and photo uploads directly from the field.

### ⏱️ Smart Attendance & Timesheets
- **Frictionless Check-in / Check-out:** One-click attendance workflow.
- **Automated Timesheets:** Calculates total daily hours and flags late or absent days.
- **Payroll Ready:** Monthly statistics formatted for easy payroll integration.

### 🗓️ Multi-Step Leave Management
- Streamlined employee request portal (Casual, Sick, Earned).
- **2-Step Approval Workflow:** Requires immediate supervisor approval followed by final HR/HOD sign-off, ensuring proper chain-of-command validation.

### 📊 Advanced Dashboards & Analytics
Powered by **Chart.js**, interactive dashboards are dynamically filtered based on the logged-in user's clearance level.
- **KPI Metrics:** Active workforce rate, pending tasks, workforce counts, and pending approvals.
- **Trend Analysis:** Sales visit velocity charts over rolling 7-day windows.
- **Workforce Distribution:** Departmental and status (Active/Leave/Inactive) distribution graphs.

### 🔄 Intelligent Bulk Import / Export Engine
- **SheetJS Integration:** Allows L6 admins to onboard hundreds of employees instantly via Excel templates.
- **Strict Data Validation:** Client-side algorithms validate data uniqueness, regex patterns (PAN/Aadhaar formats), age constraints, and dropdown limits *before* database insertion.
- **Sanitized Exports:** L5 managers exporting department lists automatically have Sensitive PII (Aadhar, Bank Details) redacted by the export engine.

### 🔒 Enterprise-Grade Security
- **Firestore Security Rules:** Read/Write operations are mathematically bound to the user's Auth Token and RBAC level. Lower-tier users are cryptographically prevented from querying unauthorized data.
- **Brute-Force Protection:** 5 consecutive failed logins trigger a strict 15-minute account lockout.
- **Mandatory Security Policies:** First-time logins are forced through a password change wizard enforcing strict complexity requirements (Uppercase, Number, Symbol, Min 8 chars).

---

### 💼 Portfolio Context
*This project highlights deep expertise in building complex, data-heavy enterprise web applications using modern serverless infrastructure. It demonstrates full-stack capabilities ranging from intuitive UI/UX design and complex client-side state management to secure NoSQL database structuring and dynamic, role-based data pipelining.*
