# Business Requirements

## Core Functionality
- **Inventory Management:** Track pharmaceutical products and pet accessories.
- **Physical Sales (POS):** Manual stock deduction for in-store sales (replacing Microchip system).
- **Online Store:** Customer-facing catalog with shopping cart.

## Legal & Fiscal
- **Tax Compliance:** Collect fiscal data for Mexican CFDI 4.0 invoicing.
- **Privacy:** Implement data protection policies according to Mexican law.

## Logistics
- **Scope:** Local delivery within Aguascalientes.

## Detailed User Stories

### 1. Delivery Logic (The 3:00 PM Rule)
**As a** Customer,
**I want** the system to automatically check the current time,
**So that** I can see if "Same-Day Delivery" is available (before 3:00 PM) or only "Next-Day Delivery" (after 3:00 PM).

### 2. POS Inventory Sync
**As a** Staff Member,
**I want** to scan a product barcode at the physical store,
**So that** the system instantly updates the stock on the website to prevent overselling.

## Style Guide (UI/UX)

### Colors
- **Brand Green (Primary):** #2D5A41 (The forest green from logo)
- **Action Green (Secondary):** #A8D08D (For buttons and icons)
- **Background:** #F4F7F5 (Off-white for clean look)

### Visual Effects
- **Main Gradient:** From #2D5A41 to #4A7C5F (Linear, 135deg). 
  *Note: Use this for the website header and hero section.*

### Typography
- **Headings:** Montserrat or Arial (Bold)
- **Body:** Open Sans or Helvetica (Regular)
