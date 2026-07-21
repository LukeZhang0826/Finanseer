# Finanseer

A full-stack personal finance dashboard for tracking income, expenses, and budgets, with interactive charts and month-over-month trend analysis.

Live: https://finanseer.netlify.app/

## Features

- KPI dashboard with revenue, expense, and operational metrics broken down by month
- Transactions table (MUI Data Grid) with sorting and pagination
- Product/spending category breakdown with recharts visualizations
- Revenue predictions: linear regression trend line projected from historical monthly KPI data

## Tech stack

**Client** (`client/`): Vite, React 18, TypeScript, MUI v5 (+ `@mui/x-data-grid`), Redux Toolkit, React Router v6, Recharts, `regression`

**Server** (`server/`): Express (ESM), MongoDB via Mongoose, helmet/cors/morgan

## Getting started

Client and server are independent npm projects.

```bash
# server
cd server
npm install
# create a .env with MONGO_URL and (optionally) PORT
npm run dev

# client
cd client
npm install
npm run dev
```

## Deployment

Client is deployed on Netlify. Server is deployed on Fly.io (`@flydotio/dockerfile`).
