# System Requirements Specification for Viv's Vintage Wear

## 1. Introduction
This document outlines the system requirements for Viv's Vintage Wear's retail management system, encompassing point of sale, customer management, and promotional operations.

## 2. Functional Requirements

### 2.1 Customer Management System
FR1.1: The system shall maintain a customer database containing:
- Customer name
- Postal address
- Email address
- Mailing preferences (postal, email, or both)

FR1.2: The system shall allow Sales Assistants to register new customers for the mailing list during purchase transactions.

FR1.3: The system shall support customer opt-in choices for promotional communications.

### 2.2 Point of Sale (POS) System
FR2.1: The system shall process the following payment methods:
- Cash payments
- Card payments
- Gift cards
- Discount cards

FR2.2: The system shall validate and process £10 discount cards:
- Verify card authenticity
- Apply discount to total purchase amount
- Record used cards for auditing

FR2.3: The system shall manage gift card transactions:
- Read gift card balances
- Deduct purchase amounts from gift cards
- Display remaining balance
- Allow split payments between gift cards and other payment methods

FR2.4: The system shall implement the Gift Your Old Gear scheme:
- Apply 15% discount to qualifying transactions
- Prevent combination with other offers
- Prevent application to gift card purchases

FR2.5: The system shall process item returns:
- Validate return eligibility (28-day window)
- Process refunds to original payment method
- Issue gift cards for returns without receipts
- Verify item condition and tags

### 2.3 Inventory Management
FR3.1: The system shall maintain real-time inventory across all store locations.

FR3.2: The system shall support inter-store inventory queries and transfers:
- Check stock availability at other locations
- Process store-to-store transfers
- Handle home delivery orders
- Calculate and apply delivery fees

### 2.4 Promotional System
FR4.1: The system shall manage promotional campaigns:
- Seasonal brochure tracking
- Email campaign management
- Special offer implementation
- Discount code application

## 3. Non-Functional Requirements

### 3.1 Performance
NFR1.1: The system shall process all POS transactions within 3 seconds.

NFR1.2: The system shall support simultaneous operations across all 20 store locations.

### 3.2 Security
NFR2.1: The system shall encrypt all customer personal data.

NFR2.2: The system shall implement role-based access control for different user types.

### 3.3 Reliability
NFR3.1: The system shall maintain 99.9% uptime during store operating hours.

NFR3.2: The system shall perform automated daily backups of all data.

### 3.4 Usability
NFR4.1: The system shall provide an intuitive interface requiring minimal training for sales staff.

NFR4.2: The system shall support efficient processing of transactions with minimal steps.

### 3.5 Maintainability
NFR5.1: The system shall be modular to allow for easy updates and modifications.

NFR5.2: The system shall maintain comprehensive transaction logs for auditing purposes.

## 4. Constraints
C1: The system must integrate with existing EPOS hardware.

C2: The system must comply with UK data protection regulations.

C3: The system must support both online and offline operations to handle internet connectivity issues.

## 5. Assumptions and Dependencies
A1: All stores have reliable internet connectivity.

A2: Staff will receive adequate training on system usage.

D1: Integration with existing payment processing systems.

D2: Compatibility with current hardware infrastructure.
