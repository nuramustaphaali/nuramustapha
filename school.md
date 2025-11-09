# 🏫 Project Name: NextGen School Management System (NextGen SMS)

## 🚀 Overview
The NextGen School Management System is a modern, high-performance web application designed to handle all administrative, academic, and financial operations for a modern Nigerian school. Built for speed and reliability, the system supports a target user load of **up to 50,000 daily visitors** and provides a responsive, mobile-app-like experience across all devices.

## ✨ Core Features & Philosophy
* **High Performance:** Decoupled architecture (Next.js Frontend + Node.js Backend) ensures rapid loading and low latency.
* **Secure RBAC:** Robust Role-Based Access Control protecting sensitive data.
* **Mobile-First Design:** Implemented as a **Progressive Web App (PWA)** for an installable, native-like user experience.
* **Nigerian Context Ready:** Integrates with local payment gateways (Paystack/Flutterwave) and supports common local result computation.

## 💻 Technology Stack
| Component | Technology | Rationale |
| :--- | :--- | :--- |
| **Frontend** | **Next.js (React)** | SSR/SSG for speed and PWA capability for mobile-like responsiveness. |
| **Backend (API)** | **Node.js (NestJS Framework)** | Non-blocking I/O for high concurrency (50k daily visitors). NestJS adds strong structure. |
| **Database** | **PostgreSQL (or MySQL)** | Chosen for data integrity and strong transactional support for financial and academic records. |
| **Payments** | **Paystack / Flutterwave SDKs** | Secure, localized online payment and reconciliation. |

---

## 🔐 System User Roles and Key Features

The system operates with six distinct roles, each with defined access limitations to ensure security and data integrity.

### 1. 👑 Principal / Super Admin (Management & Global Control)
| Feature Module | Key Responsibilities |
| :--- | :--- |
| **Website Settings** | **CRUCIAL:** Change School Name, Logo, Address, Contact Details, Official Email, and Footer Text. Configure Default Grading Scales. |
| **Academics** | Change/Lock **Session** & **Term**. Create, Edit, and Archive Classes/Arms. Promote students. |
| **User Management** | Full control: Create, edit, and deactivate all staff and bursar accounts. Assign **Form Masters**. |
| **Reporting** | Full view of Revenue, Expenses, Debtor Reports, and **School Performance Analytics**. |
| **Document Control**| Full access to **print ALL vital documents** (e.g., Admission Letters, Staff Contracts, Student Transcripts). |

### 2. 👨‍🏫 Teacher / Form Master (Academic Operations)
| Feature Module | Key Responsibilities |
| :--- | :--- |
| **Result Entry** | Enter **Continous Assessment (CA)** and **Exam Scores** for assigned subjects/classes. |
| **Attendance** | Mark daily student attendance in **real-time** (with PWA offline-sync capability). |
| **Class Management** | **Form Master:** Approve and Publish termly results for their assigned class. Track behavior/demeanor. |
| **Communication** | Send instant notes/updates to parents of their assigned students. |

### 3. 💰 Bursar / Accountant (Financial Operations)
| Feature Module | Key Responsibilities |
| :--- | :--- |
| **Fee Management** | Set Fees/Levies, track Payments/Arrears, and generate payment receipts. |
| **Invoicing** | Generate digital/printable **Student Bills** (Invoices). Send **SMS Alerts** for overdue fees. |
| **Reconciliation** | Record offline cash payments and reconcile online transactions via payment gateway reports. |

### 4. 👨‍🎓 Student (Information Access)
| Feature Module | Key Access Points |
| :--- | :--- |
| **Dashboard** | View Attendance Record, Current Class/Session, and Announcements. |
| **Academics** | View and **download official Termly Report Cards** and **Academic Transcript** history. |
| **Finance** | View personal Fee Status and Payment History. Direct link to payment portal. |

### 5. 👨‍👩‍👧 Parent (Monitoring & Engagement)
| Feature Module | Key Access Points |
| :--- | :--- |
| **Child Monitoring** | View Real-Time Attendance and Behavior Reports for multiple children (Single Login). |
| **Academics** | View **Official Termly Results** for their children once published by the Form Master. |
| **Finance** | View outstanding Bills, make **Online Payments** via Paystack/Flutterwave, and download receipts. |

---

## 📄 Critical Document Printing & Export

All users with appropriate permissions (Admin, Staff, Student) must be able to print vital documents seamlessly.

* **Technology Implementation:** Dedicated PDF generation services will ensure professional, non-broken layouts suitable for official records.
* **Key Printable Documents:**
    * **Student Records:** Admission Letter, Termly Report Card, Academic Transcript, School ID Card.
    * **Financial:** Student Invoices/Bills, Payment Receipts, Fee Defaulters List.
    * **Administrative:** Staff Contracts, Class Lists, Teacher Timetables***
