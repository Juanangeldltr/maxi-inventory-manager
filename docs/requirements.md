# Business Requirements & System Logic

## Core Functionality
- **Inventory Management:** Track pharmaceutical products and pet accessories.
- **Physical Sales (POS):** Manual stock deduction for in-store sales (replacing Microchip system).
- **Online Store:** Customer-facing catalog with shopping cart.

## Legal & Fiscal
- **Tax Compliance:** Collect fiscal data for Mexican CFDI 4.0 invoicing.
- **Privacy:** Implement data protection policies according to Mexican law.

## Logistics
- **Scope:** Local delivery within Aguascalientes.

---

## Detailed User Stories (For Team Collaboration)

### 1. Delivery Logic (The 3:00 PM Rule)
**As a** Customer,
**I want** the system to automatically check the current time,
**So that** I can see if "Same-Day Delivery" is available (before 3:00 PM) or only "Next-Day Delivery" (after 3:00 PM).

### 2. POS Inventory Sync
**As a** Staff Member,
**I want** to scan a product barcode at the physical store,
**So that** the system instantly updates the stock on the website to prevent overselling.

---

## Technical Logic & Flowcharts

### A. Same-Day Delivery Decision Tree
1. **Start:** Customer views shopping cart.
2. **System Check:** Get current system time (Aguascalientes).
3. **Condition:** Is current time < 15:00 (3:00 PM)?
    - **YES:** Display "Express Delivery Available (Today)" + Priority Fee.
    - **NO:** Display "Standard Delivery (Tomorrow)".
4. **End:** Checkout process continues with selected delivery date.



### B. POS Stock Update Flow
1. **Action:** Scan product barcode in physical store.
2. **Lookup:** Find matching ID in `src/data/products.json`.
3. **Calculation:** `stock = stock - 1`.
4. **Validation:** If `stock <= 3`, trigger "Low Stock" alert for manager.
5. **Sync:** Update the web catalog view instantly.



---

## Style Guide (UI/UX)

### Colors
- **Brand Green (Primary):** #2D5A41 (Forest Green from logo)
- **Action Green (Secondary):** #A8D08D (For buttons and icons)
- **Background:** #F4F7F5 (Off-white for clean look)

### Visual Effects
- **Main Gradient:** linear-gradient(135deg, #2D5A41, #4A7C5F)
  *Note: Use for website header and hero sections.*

### Typography
- **Headings:** Montserrat or Arial (Bold)
- **Body:** Open Sans or Helvetica (Regular)

---
## Website Sitemap (Navigation Structure)

Based on the brand identity, the navigation bar will include:

1.  **Inicio (Home):** General overview and welcome.
2.  **Productos (Products):** Main catalog (Pharmacy and Accessories).
3.  **Ofertas (Offers):** Special discounts and seasonal promotions.
4.  **Contacto (Contact):** WhatsApp link and clinic location.
5.  **Sobre nosotros (About Us):** The clinic's history and family values.
6.  **Cuenta (Account):** Client login and order history.

**Key Icons:**
- Shopping Cart (Direct access to checkout).
- Location (Link to Google Maps/Aguascalientes branch).
- Profile/Account (User management).
