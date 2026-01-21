# Project Proposal: Maxi Inventory Manager

## 1. Direct Savings & Independence
The current systems (like Microchip) often involve expensive licenses or recurring fees. This custom-developed solution will have **$0 maintenance costs** for licenses. The system will run locally on existing hardware, utilizing the current Point Smart terminal and barcode scanners.

## 2. Local-First Reliability (Offline Operations)
Unlike web-based systems, this application will be built using **Tauri and SQLite**. This means:
- **100% Uptime:** The clinic can sell and manage stock even if the internet provider fails.
- **Speed:** Instant response times as data doesn't need to travel to a cloud server.

## 3. Unified Management (The "Single Window" Strategy)
We will eliminate the inefficiency of switching between three different windows for sales, purchases, and reception. All core business logic will be integrated into a single, streamlined React interface.

## 4. Automated Fiscal Integration
The system will handle **SAT CFDI 4.0 invoicing** directly. By automating the fetching of costs from the latest purchase records and integrating a fiscal API, we reduce human error and save time during the checkout process.

## 5. Security & User Control
A role-based login system will ensure that only authorized personnel can access sensitive financial reports or modify product costs, providing the owners with full control over their business data.
