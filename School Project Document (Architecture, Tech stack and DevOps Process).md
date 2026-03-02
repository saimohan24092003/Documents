# Architecture


# Architecture Stack

## Frontend

| Technology | Version | Purpose |
|------------|---------|---------|
| Next.js | 14.2.2 | Full-stack React framework, App Router |
| React | 18 | UI component library |
| TypeScript | v5 | Type-safe JavaScript |
| Tailwind CSS | v3.4 | Utility-first styling |
| Radix UI | v1 | Accessible headless UI components (Dialog, Avatar, Progress) |
| Lucide React | v0.383 | Icons |
| Zustand | v4.5 | Client-side state (modal open/close) |
| Sonner | v1.4 | Toast notifications |
| React Confetti | v6.1 | Celebration animation on completion |

---

## Backend

| Technology | Version | Purpose |
|------------|---------|---------|
| Next.js API Routes | 14.2.2 | Serverless API endpoints |
| Next.js Server Actions | 14.2.2 | Direct server functions (exam submit, grading) |
| Drizzle ORM | v0.31 | Type-safe database queries |
| Node.js | v20+ | Runtime |

---

## Database

| Technology | Version | Purpose |
|------------|---------|---------|
| Neon PostgreSQL | Serverless | Primary database (scales to zero) |
| @neondatabase/serverless | v0.9.3 | HTTP connector for Neon |

---

## Authentication

| Technology | Version | Purpose |
|------------|---------|---------|
| Clerk | v5.0.5 | Full auth — sign-in, sign-up, session, user management |

---
## Deployment Flow — Local to Live (Vercel)

## Step 1 — You wrote code on your laptop

```bash
pnpm dev
```

* Only you could see it at `http://localhost:3000`
* Nobody else in the world could access it.

---

## Step 2 — You pushed to GitHub

```bash
git add .
git commit -m "your message"
git push origin main
```

* Your code is now safely stored on GitHub.
* Still not live for users yet.

---

## Step 3 — Vercel detected the push

Vercel watches your GitHub repository automatically.

When you push:

* Vercel pulls your code
* Runs:

```bash
pnpm build
```

* Builds your production-ready application.

---

## Step 4 — Vercel made it live

Vercel deploys your app to global servers.

When anyone opens your URL:

* Vercel serves the page
* Website loads in milliseconds worldwide.

---

## Flow Summary

```
Your Laptop
     ↓
GitHub Repository
     ↓
Vercel Auto Build
     ↓
Live Website (Worldwide)
```

