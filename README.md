# Department Library Management System

A web‑based application designed to digitize and streamline academic library operations within your IT department. Developed as part of UIT2402 – Advanced Data Structures & Algorithm Analysis, this system leverages advanced data structures and secure web practices to enhance search performance, automate workflows, and improve user experience for both library staff and patrons.

---

## 🚀 Project Overview

Traditional departmental library systems often struggle with slow searches, manual record‑keeping, and limited user roles. This project solves those pain points by offering:

* **Fast, intelligent search** via a Trie‑based autocomplete engine for instant suggestions.
* **Role‑based dashboards** for Admins and Students/Faculty, minimizing unauthorized access.
* **End‑to‑end book management**: catalog CRUD, borrowing/return workflows, and real‑time availability updates.
* **Automated notifications** for due dates and overdue items to reduce manual follow‑up.
* **Scalable, modular architecture** built on RESTful APIs and optimized database indexing.

---

## 🎯 Core Features

### 1. Secure User Management

* **Role-Based Access Control**: Distinct **Admin** and **Student/Faculty** roles with permissions tailored to each group:

  * **Admins** can manage books, user accounts, and approve or reject borrow requests.
  * **Students/Faculty** can browse the catalog, submit borrow/return requests, and view personal history.
* **Authentication & Security**:

  * Passwords stored with industry-standard hashing (bcrypt).
  * Email verification workflow for new accounts.
  * Session management via secure cookies or JWT tokens with configurable expiration.

### 2. Advanced Search & Autocomplete

* **Trie Data Structure**:

  * Provides **O(L)** lookup time for prefix matches, where *L* is the query length.
  * Reduces memory overhead by sharing common prefixes across entries.
* **Dynamic Filtering & Sorting**:

  * Filter results by categories (e.g., Programming, Networking, Databases) and availability status.
  * Sort by relevance, title, author name, or date of entry.
* **Error Tolerance**:

  * Suggests closest matches for minor typos or incomplete queries.

### 3. Comprehensive Catalog Management

* **CRUD Operations**:

  * Add new books with metadata: title, author, ISBN, category, shelf number, and acquisition date.
  * Update book details or remove outdated entries.
* **Bulk Import/Export**:

  * CSV/Excel import for large datasets in one operation.
  * Export catalog snapshots for offline analysis.
* **Availability Tracking**:

  * Real‑time status updates when books are borrowed or returned.
  * Automatic count of total and available copies.

### 4. Borrowing & History Tracking

* **Borrow/Return Workflow**:

  * Students submit requests through the interface.
  * Admins receive a dashboard notification and can approve or deny with optional notes.
* **Due Date Logic**:

  * Configurable loan periods (e.g., 14 days by default).
  * Automatic accrual of fines for overdue items, with rate and maximum caps.
* **Audit Trail**:

  * Complete transaction logs detailing timestamps, user IDs, and admin actions for compliance.

### 5. Notifications & Reminders

* **Email Alerts**:

  * Scheduled reminders sent 3 days before due date and on the morning of the due date.
  * Overdue notices dispatched daily until the book is returned.
* **In‑App Notifications**:

  * Dashboard banners highlight items nearing due dates or already overdue.
* **Custom Templates**:

  * Admins can modify email subject lines and message bodies without code changes.

---

## 💡 Use Cases

* **Library Staff (Admins)**: Efficiently manage inventory, process borrow requests, and monitor overdue returns with minimal manual effort.
* **Students & Faculty**: Rapidly locate and reserve books, track personal loan history, and receive timely reminders.
* **Department Heads**: Analyze usage trends and resource allocation through built‑in reporting modules.

---

## 🧱 Tech Stack

**Frontend**

* HTML, CSS, JavaScript
  
**Backend**

* Python & Flask
* PostgreSQL

**Data Structures & Algorithms**

* **Trie** for autocomplete (efficient prefix searching)

---

## Screenshots

* Login
![image](https://github.com/user-attachments/assets/96501eba-2e05-4b84-ac27-6b8737e577a7)

* User side
![image](https://github.com/user-attachments/assets/8927cee5-50f8-43ed-938c-17b057957107)
![image](https://github.com/user-attachments/assets/17e0ec38-93ed-4b86-ae23-1e6def2f390b)
![image](https://github.com/user-attachments/assets/8b10b4ec-2c86-48ed-9416-2a03a943f38f)
![image](https://github.com/user-attachments/assets/cd2e6af0-902c-493b-8743-9d66cdc79893)
![image](https://github.com/user-attachments/assets/82239e68-9723-4725-afc1-cb0c60c85b25)
![image](https://github.com/user-attachments/assets/0a16963c-eea1-4d0f-a496-7c4da6f7cfde)

* Admin side
![image](https://github.com/user-attachments/assets/787d3c07-8096-4e30-a299-7db9160f0916)
![image](https://github.com/user-attachments/assets/db8702ec-ca91-423c-b2fd-05d14295b9e6)
![image](https://github.com/user-attachments/assets/058e80d2-bbc9-49cc-b522-1907dc11b3f7)

---

## 🔮 Future Scope

* **External Metadata Integration**: Sync with global book databases (e.g., ISBN registries) for automatic metadata enrichment.
* **Recommendation Engine**: Machine‑learning‑powered suggestions based on borrowing history and user preferences.
* **Mobile App**: Native or hybrid application for on‑the‑go catalog access and mobile checkout.
* **Analytics Dashboard**: Visual charts and heatmaps showing peak usage times and popular titles.
* **Barcode & RFID Scanning**: Streamlined check‑in/check‑out with hardware integration.
* **Enhanced Security**: Multi‑factor authentication and role‑based session policies.

