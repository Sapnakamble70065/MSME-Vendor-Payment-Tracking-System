# MSME Vendor Payment Tracking System

A backend API system designed for MSMEs to efficiently manage vendors, purchase orders,
and vendor payments. The system helps track outstanding balances, payment statuses,
and provides analytics to support better working capital management.

This project is developed as part of the **Back-End Developer Intern Assignment** for QistonPe.

---

## 🚀 Tech Stack

- Backend Framework: NestJS (TypeScript)
- Database: PostgreSQL
- ORM: Prisma
- Authentication: JWT
- Validation: class-validator
- API Documentation & Testing: Postman
- Deployment: Railway / Render

---

## 📦 Features

### Must-Have Features
- Vendor Management API
- Purchase Order Management
- Auto-generated PO numbers
- Payment Recording with PO status auto-update
- Outstanding amount calculation
- Vendor outstanding analytics
- DTO validation & proper error handling

### Nice-to-Have Features
- JWT-based authentication
- Soft delete for payments
- Pagination on list APIs
- Seed data for testing

---

## ⚙️ Setup Instructions

### Prerequisites
Ensure the following are installed:
- Node.js (v18 or higher)
- npm
- PostgreSQL

---

### Installation Steps

Clone the repository:
```bash
git clone <YOUR_GITHUB_REPO_URL>
cd msme-vendor-payment-system

 🔐 Environment Variables

Create a .env file using .env.example.
DATABASE_URL=postgresql://username:password@localhost:5432/msme_db
JWT_SECRET=your_jwt_secret
PORT=3000

▶️ Running the Application
🧩 Database Schema
Tables

vendors

purchase_orders

purchase_order_items

payments

users

Relationships

Vendor → Purchase Orders (One-to-Many)

Purchase Order → Payments (One-to-Many)

Purchase Order → Items (One-to-Many)

🔑 Authentication
Login API
POST /auth/login


Request Body:

{
  "email": "admin@qistonpe.com",
  "password": "admin123"
}


Response:

{
  "access_token": "JWT_TOKEN"
}


Use this token in Postman:
Authorization → Bearer Token → Paste JWT token.

All protected APIs require this token.

📡 API Endpoints
Vendors

POST /vendors

GET /vendors

GET /vendors/:id

PUT /vendors/:id

Purchase Orders

POST /purchase-orders

GET /purchase-orders

GET /purchase-orders/:id

PATCH /purchase-orders/:id/status

Payments

POST /payments

GET /payments

GET /payments/:id

DELETE /payments/:id (soft delete)

Analytics

GET /analytics/vendor-outstanding


📊 Business Logic

PO total amount is calculated from line items

Due date auto-calculated using vendor payment terms

Payment amount cannot exceed outstanding amount

PO status auto-updates:

Approved → Partially Paid → Fully Paid

Outstanding = PO Total − Sum of all payments


🧪 Testing the API (Main Flow)

Login and get JWT token

Create Vendor

Create Purchase Order

Make partial payment → PO status becomes Partially Paid

Make remaining payment → PO status becomes Fully Paid

Attempt overpayment → API returns validation error


