# 🧾 Kodein Billing System

> A billing, subscription, and invoicing management platform built during my time at **Kodein** — an Indonesian IT company that designs, develops, and hosts websites and mobile applications for businesses across Indonesia.

## 📸 Screenshots

| Login | Dashboard | Billing |
|---|---|---|
| <img src="screenshots/login.png" width="220"/> | <img src="screenshots/dashboard.png" width="220"/> | <img src="screenshots/billing.png" width="220"/> |

| Orders | Subscriptions | Products |
|---|---|---|
| <img src="screenshots/orders.png" width="220"/> | <img src="screenshots/subscriptions.png" width="220"/> | <img src="screenshots/products.png" width="220"/> |

> Screenshots are also available in the [`screenshots/`](screenshots/) folder for a closer look.

---

## 🎯 What It Is

**Kodein Billing System** is an internal SaaS that gives Kodein one place to manage the full lifecycle of a client project — from order approval and progress tracking, to recurring subscriptions and invoicing.

It replaces the manual, spreadsheet-based workflow with a single dashboard where the team can see what is in progress, what needs approval, and what is due for payment — all in real time.

> **Demo build.** All data shown in this demo is sample data for illustrative purposes only. This is a documentation copy of the system.

---

## ✨ Features

- 📦 **Project Management** — create and approve project orders with configurable down payments, track progress milestones, and attach files along the way
- 🔁 **Subscription Management** — recurring subscriptions with weekly / monthly / annual billing periods, automatic renewal tracking, and a full grace-period → suspension → re-billing lifecycle
- 💳 **Billing & Payments** — automatic bill generation, invoice and proof-of-payment uploads, approve / decline / refund (credit note) workflows, and tax support
- 📄 **Invoice PDF** — generate a clean, secure invoice PDF on demand
- 🔔 **Notifications** — in-app alerts for approvals, renewals, and expiring bills
- 👥 **Role-based Access** — Superadmin, Admin, Marketing, Finance, Client, and a read-only Viewer role

---

## 🛠 Built With

- ⚛️ **Next.js** — App Router, React, TypeScript
- 🎨 **Tailwind CSS** — UI styling
- 🗄️ **Supabase** — PostgreSQL database and private file storage
- 🔐 **JWT** — access + rotating refresh tokens with httpOnly cookies
- 📧 **Nodemailer** — email reminders (fictional `@example.com` addresses in this demo)
- ☁️ **Vercel** — serverless hosting and scheduled cron jobs

---

## 🚀 Live Demo

Open the live demo: **[https://kodein-billing-system.vercel.app](https://kodein-billing-system.vercel.app)**

| Role | Email | Password | Access |
|---|---|---|---|
| Viewer | `viewer@example.com` | `Demo@123` | Read-only across every module |
| Finance | `finance@example.com` | `Demo@123` | Payments, bills, invoices |
| Marketing | `marketing@example.com` | `Demo@123` | Orders and progress |
| Client | `client@example.com` | `Demo@123` | Own bills and orders |

> 🔒 The **Superadmin** and **Admin** accounts are intentionally **not** listed here — they are reserved for internal management and use strong, unique passwords.

---

## 🔒 Security

- JWT authentication with httpOnly, secure cookies and rotating refresh tokens
- Role-based access enforced on **every API route**, not just the UI
- Private storage bucket — files are only reachable through an authenticated proxy
- On-demand PDF generation — invoices are never stored as files
- Rate limiting on auth, upload, and PDF endpoints
- Parameterized SQL (injection-safe) and hardened security headers

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Melvin** ([@CodeMelvin](https://github.com/CodeMelvin))
