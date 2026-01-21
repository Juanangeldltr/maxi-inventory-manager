# System Requirements - Maxi Inventory Manager

## General Objective
Develop a local Point of Sale (POS) and Inventory Management system to unify veterinary operations into a single, agile interface, eliminating dependency on slow legacy software.

## Core Functionality (Offline-First)
- **Unified Management:** Control of Sales, Purchases, and Stock Reception in a single view (replacing the current 3-window system).
- **Detailed Kárdex:** Complete movement history per item to validate refunds, invoice numbers, and applied pricing.
- **Tax Compliance Module:** Mandatory fields for Mexican SAT product codes, Tax Regime, and CFDI usage.

## Business Logic & Automation
- **Cost Automation:** The system must automatically fetch the "Minimum Purchase Price" based on the latest recorded purchase (eliminating manual entry).
- **Profit Calculation:** Daily, weekly, and monthly reports based on (Sales Price - Purchase Cost), minus commissions.
- **Payment Methods:** Cash, Debit Card, and Credit Card (Check payments are removed).

## Output & Printing
- **Physical Documents:** Optional sales tickets and "Purchase Order" reports (stock needed from providers).
- **Invoicing:** Electronic invoice (CFDI) generation meeting all SAT requirements upon customer request.
