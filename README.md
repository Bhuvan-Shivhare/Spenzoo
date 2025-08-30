# 💸 Spenzo – Smarter Money, Powered by AI

<div align="center">
  <img src="public/logo.png" alt="Spenzo Logo" width="200"/>

  <br/>

  [![Live Demo](https://img.shields.io/badge/Live_Demo-View_Now-22c55e?style=for-the-badge&logo=vercel)](https://spenzo.vercel.app/)
  [![Next.js](https://img.shields.io/badge/Next.js-15.4.4-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
  [![React](https://img.shields.io/badge/React-19.0.0-blue?style=for-the-badge&logo=react)](https://reactjs.org/)
  [![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
  [![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4.1-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)
  [![Prisma](https://img.shields.io/badge/Prisma-6.0.1-2D3748?style=for-the-badge&logo=prisma)](https://www.prisma.io/)
  [![PostgreSQL](https://img.shields.io/badge/PostgreSQL-13+-336791?style=for-the-badge&logo=postgresql)](https://www.postgresql.org/)
  [![Clerk](https://img.shields.io/badge/Clerk-Auth-6C47FF?style=for-the-badge)](https://clerk.com/)
  [![Google AI](https://img.shields.io/badge/Google_AI-Gemini-4285F4?style=for-the-badge)](https://ai.google.dev/)
</div>

---

## 🌐 Live Demo

**Explore Spenzo in action:** [https://spenzo.vercel.app](https://spenzo.vercel.app)  
Experience the future of personal finance — from AI-driven budgeting to smart receipt scanning.

---

## 🧠 What is Spenzo?

**Spenzo** is an AI-powered personal finance platform designed to simplify money management. With advanced machine learning and modern UI/UX, it automates the boring stuff so you can focus on financial freedom.

From tracking expenses and managing budgets to extracting data from receipts using Google’s Generative AI — Spenzo does it all, intelligently.

---

## ✨ Features at a Glance

### 💼 Money Management
- **All Accounts, One Dashboard** – View and manage multiple bank accounts
- **Automatic Categorization** – Know where your money goes, effortlessly
- **Smart Budgeting** – Get tailored budget recommendations
- **Real-time Updates** – Stay up-to-date with live account balances
- **Recurring Payment Handling** – No more surprises on your statement

### 🤖 AI-Powered Intelligence
- **AI Receipt Scanner** – Upload a receipt, we’ll handle the rest
- **Auto Categorization** – AI classifies your transactions with precision
- **Insightful Analytics** – Get meaningful suggestions based on your habits
- **Predictive Budgeting** – Forecast spending trends

### 📱 Seamless User Experience
- **Sleek Interface** – Built with Tailwind CSS & Radix UI
- **Responsive Design** – Perfect across all devices
- **Dark Mode / Light Mode** – Your preference, respected
- **Smooth Navigation** – Designed for clarity and usability

### 🔐 Security & Infrastructure
- **Secure Auth with Clerk** – Protecting your data at every step
- **Rate Limiting with ArcJet** – Prevent abuse & ensure reliability
- **Zod Validation** – Keeping inputs clean & safe
- **Turbopack** – Lightning-fast build times

---

## 🔧 Tech Stack

| Layer        | Technologies |
|--------------|--------------|
| **Frontend** | Next.js 15, React 19, Tailwind CSS, Radix UI, Lucide Icons |
| **Backend**  | Prisma, PostgreSQL, Inngest, ArcJet |
| **AI/Services** | Google Generative AI, Resend, Clerk |
| **Dev Tools** | ESLint, Turbopack, PostCSS |

---

## 🗃️ Database Overview

Spenzo uses a PostgreSQL database with Prisma ORM. Here's a brief overview:

- **User** – Auth, profiles, and linked accounts
- **Account** – Current & Savings with balance sync
- **Transaction** – Categorized, recurring, and scanned receipts
- **Budget** – Custom limits, alerts, and analytics

---

## 🚀 Getting Started

### ✅ Requirements
- Node.js 18+
- PostgreSQL
- Clerk Account
- Google AI Key
- Resend API Key

### 📦 Installation Steps

```bash
git clone https://github.com/WaliKhan09/spenzo.git
cd spenzo
npm install


# DB
DATABASE_URL=postgresql://username:password@localhost:5432/spenzo

# Clerk Auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=...
CLERK_SECRET_KEY=...

# Google AI
GEMINI_API_KEY=...

# Email
RESEND_API_KEY=...

# ArcJet
ARCJET_KEY=...

# Inngest
INNGEST_EVENT_KEY=...
INNGEST_SIGNING_KEY=...


npx prisma generate
npx prisma db push
npm run seed

spenzo/
├── app/                  # Routes & Pages
│   ├── (auth)/           # Auth screens
│   ├── (main)/           # Dashboard & features
│   └── api/              # API routes
├── components/           # UI components
├── lib/                  # Utility & helper functions
├── prisma/               # Database models
├── actions/              # Server actions
├── emails/               # Email templates
├── public/               # Static assets

