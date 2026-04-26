# Welth - AI Finance Platform

Welth is a full-stack personal finance platform that helps users track accounts, categorize transactions, set budgets, and receive AI-powered financial insights.

## Features

- Secure authentication with Clerk
- Account and transaction management
- Budget tracking and alerting
- AI receipt scanning and smart insights with Gemini
- Background jobs for recurring workflows with Inngest
- Email notifications with Resend
- Rate limiting and bot protection with ArcJet

## Tech Stack

- Next.js (App Router)
- React + Tailwind CSS + shadcn/ui
- Prisma ORM
- Supabase Postgres
- Clerk
- Inngest
- Google Gemini API
- Resend
- ArcJet

## Environment Variables

Create a `.env` file in the project root:

```bash
DATABASE_URL=
DIRECT_URL=

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard

GEMINI_API_KEY=

RESEND_API_KEY=

ARCJET_KEY=
```

## Local Setup

```bash
npm install
npx prisma migrate deploy
npm run dev
```

App runs at `http://localhost:3000`.

## Deployment

Deploy on Vercel and add the same environment variables in the Vercel project settings.
