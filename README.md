# Maxi Inventory Manager

Professional inventory management and Point of Sale (POS) system developed for **MAXI VETERINARIA**.

## Project Overview
A robust **offline-first** desktop application built with **Tauri**. It replaces legacy software with a high-performance interface to manage sales, inventory, and automated SAT invoicing. The system is designed to work without an internet connection, syncing fiscal data only when needed.

## Key Features
- **Integrated POS:** Full offline operations including stock management and real-time sales tracking.
- **Local Database:** Powered by **SQLite** for secure, fast, and serverless data storage directly on the clinic's computer.
- **Role-Based Access Control (RBAC):** Customizable user permissions. Admins can restrict access to profit reports, cost editing, and sensitive data.
- **Fiscal & Print Engine:** - Automated SAT CFDI 4.0 invoicing (Queue-based: syncs when internet is available).
  - Thermal ticket printing and "Purchase Order" report generation.
- **Smart Cost Automation:** Automatic "Minimum Purchase Price" updates based on the latest stock reception.

## Tech Stack
- **Frontend:** React.js (User Interface).
- **Desktop Framework:** Tauri (Rust-based, lightweight and secure).
- **Database:** SQLite (Local storage).
- **Styling:** CSS3 / Tailwind (Clean and professional UX).

## Architecture Approach
The application follows a **Local-First** architecture. This ensures that the veterinary clinic can continue its daily operations (sales, inventory lookups, and reports) even during internet outages, maintaining 100% uptime for core business processes.

---
*Status: Currently in Documentation & Requirement Analysis Phase.*
