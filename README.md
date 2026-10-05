# Alfarma Cosmetics Stores

Multi-store cosmetics inventory/POS and customer-ordering foundation.

## Stores
1. Cantoment Store
2. International Market — Besides Former Unity Bank Store
3. International Market — Shop No. 2, Block B, Near Main Gate
4. 200 Unit Osuku Plaza — Alfarma Essential Cosmetics Store
5. Felele Branch
6. Coming Soon (inactive until activated)

## Included
- One common customer storefront
- Pickup-store selection
- Retail and wholesale product fields
- VIP/wholesale registration and approval status
- Store inventory model
- Orders/payment status model
- Audit logs
- Stock reservation fields
- Batch/expiry tracking
- PostgreSQL schema
- Express API foundation
- GitHub Pages workflow for the frontend
- PWA manifest

## Important
This is a complete project foundation, not a production-ready payment/backend deployment. Before commercial use, configure secure authentication, HTTPS, PostgreSQL hosting/backups, payment verification, WhatsApp Business API, rate limiting, secrets, monitoring and privacy/legal requirements.

## Local development
`docker compose up -d db`
`cd server && npm install`
Copy `.env.example` to `.env`, set secure values, then:
`npm run db:init`
`npm run db:seed`
`npm run dev`

Open `http://localhost:3000`.

Demo accounts: `admin1 / ChangeMe123!` and `admin2 / ChangeMe456!`. Change them before real use.

GitHub Pages publishes the `web` folder only. The secure API/database must be hosted separately.
