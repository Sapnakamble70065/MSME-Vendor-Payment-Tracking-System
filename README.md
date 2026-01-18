<<<<<<< HEAD
<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <p align="center">A progressive <a href="http://nodejs.org" target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>
    <p align="center">
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/dm/@nestjs/common.svg" alt="NPM Downloads" /></a>
<a href="https://circleci.com/gh/nestjs/nest" target="_blank"><img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" /></a>
<a href="https://discord.gg/G7Qnnhy" target="_blank"><img src="https://img.shields.io/badge/discord-online-brightgreen.svg" alt="Discord"/></a>
<a href="https://opencollective.com/nest#backer" target="_blank"><img src="https://opencollective.com/nest/backers/badge.svg" alt="Backers on Open Collective" /></a>
<a href="https://opencollective.com/nest#sponsor" target="_blank"><img src="https://opencollective.com/nest/sponsors/badge.svg" alt="Sponsors on Open Collective" /></a>
  <a href="https://paypal.me/kamilmysliwiec" target="_blank"><img src="https://img.shields.io/badge/Donate-PayPal-ff3f59.svg" alt="Donate us"/></a>
    <a href="https://opencollective.com/nest#sponsor"  target="_blank"><img src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg" alt="Support us"></a>
  <a href="https://twitter.com/nestframework" target="_blank"><img src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow" alt="Follow us on Twitter"></a>
</p>
  <!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)
  [![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Project setup

```bash
$ npm install
```

## Compile and run the project

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Run tests

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Deployment

When you're ready to deploy your NestJS application to production, there are some key steps you can take to ensure it runs as efficiently as possible. Check out the [deployment documentation](https://docs.nestjs.com/deployment) for more information.

If you are looking for a cloud-based platform to deploy your NestJS application, check out [Mau](https://mau.nestjs.com), our official platform for deploying NestJS applications on AWS. Mau makes deployment straightforward and fast, requiring just a few simple steps:

```bash
$ npm install -g @nestjs/mau
$ mau deploy
```

With Mau, you can deploy your application in just a few clicks, allowing you to focus on building features rather than managing infrastructure.

## Resources

Check out a few resources that may come in handy when working with NestJS:

- Visit the [NestJS Documentation](https://docs.nestjs.com) to learn more about the framework.
- For questions and support, please visit our [Discord channel](https://discord.gg/G7Qnnhy).
- To dive deeper and get more hands-on experience, check out our official video [courses](https://courses.nestjs.com/).
- Deploy your application to AWS with the help of [NestJS Mau](https://mau.nestjs.com) in just a few clicks.
- Visualize your application graph and interact with the NestJS application in real-time using [NestJS Devtools](https://devtools.nestjs.com).
- Need help with your project (part-time to full-time)? Check out our official [enterprise support](https://enterprise.nestjs.com).
- To stay in the loop and get updates, follow us on [X](https://x.com/nestframework) and [LinkedIn](https://linkedin.com/company/nestjs).
- Looking for a job, or have a job to offer? Check out our official [Jobs board](https://jobs.nestjs.com).

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://twitter.com/kammysliwiec)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](https://github.com/nestjs/nest/blob/master/LICENSE).
=======
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

### 🔐 Environment Variables

Create a .env file using .env.example.
DATABASE_URL=postgresql://username:password@localhost:5432/msme_db
JWT_SECRET=your_jwt_secret
PORT=3000
---

▶️** Running the Application**
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
---

🔑 Authentication
Login API
POST /auth/login

---

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
---

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


>>>>>>> ea842a93394a2d8d9d89f1d52d8024efcef952d7
