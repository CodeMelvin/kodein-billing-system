# ≡ƒº╛ Kodein Billing System

> A billing, subscription, and invoicing management platform built during my time at **Kodein**.

## ≡ƒô╕ Screenshots

| Login | Dashboard | Billing |
|---|---|---|
| <img src="screenshots/login.png" width="220"/> | <img src="screenshots/dashboard.png" width="220"/> | <img src="screenshots/billing.png" width="220"/> |

| Orders | Subscriptions | Products |
|---|---|---|
| <img src="screenshots/orders.png" width="220"/> | <img src="screenshots/subscriptions.png" width="220"/> | <img src="screenshots/products.png" width="220"/> |

> Screenshots are also available in the [`screenshots/`](screenshots/) folder for a closer look.

---

## ≡ƒÄ» What Is Kodein Billing System

Kodein Billing System is an internal platform that gives the team one place to manage the full lifecycle of a client project ΓÇö from order approval and progress tracking, to recurring subscriptions and invoicing.

It replaces a manual, spreadsheet-based workflow with a single dashboard where the team can see what is in progress, what needs approval, and what is due for payment ΓÇö all in real time.

> **Demo build.** All data shown is sample data for illustrative purposes only.

---

## ≡ƒÅó Why This Was Built

This platform was developed to support the internal operations of [**Kodein**](https://kodein.co.id) ΓÇö an Indonesian IT company that designs, develops, and hosts websites and mobile applications for businesses across Indonesia. See [Kodein's portfolio](https://kodein.co.id/portofolio) for examples of the company's work.

---

## Γ£¿ Features

- ≡ƒôª **Project Management** ΓÇö create and approve project orders with configurable down payments, track progress milestones, and attach files along the way
- ≡ƒöü **Subscription Management** ΓÇö recurring subscriptions with weekly / monthly / annual billing periods, automatic renewal tracking, and a full grace-period ΓåÆ suspension ΓåÆ re-billing lifecycle
- ≡ƒÆ│ **Billing & Payments** ΓÇö automatic bill generation, invoice and proof-of-payment uploads, approve / decline / refund (credit note) workflows, and tax support
- ≡ƒôä **Invoice PDF** ΓÇö generate a clean, secure invoice PDF on demand
- ≡ƒöö **Notifications** ΓÇö in-app alerts for approvals, renewals, and expiring bills
- ≡ƒæÑ **Role-based Access** ΓÇö roles for admin, finance, marketing, client, and a read-only viewer

---

## ≡ƒ¢á Built With

- ΓÜ¢∩╕Å **Next.js** ΓÇö App Router, React, TypeScript
- ≡ƒÄ¿ **Tailwind CSS** ΓÇö UI styling
- ≡ƒùä∩╕Å **PostgreSQL** ΓÇö relational database
- ≡ƒöÉ **JWT** ΓÇö secure session handling with rotating tokens
- Γÿü∩╕Å **Vercel** ΓÇö hosting and scheduled jobs

---

## ≡ƒÜÇ Live Demo

Open the live demo: **[https://kodein-billing-system.vercel.app](https://kodein-billing-system.vercel.app)**

One account is open for public testing, and it is read-only:

| Role | Email | Password |
|---|---|---|
| Viewer | `viewer@example.com` | `Demo@123` |

The viewer can browse every module but cannot create, edit, delete, approve, or upload anything.

### ≡ƒæÑ Roles

The system supports five roles besides the viewer. Credentials for these roles are deliberately not published; they belong to the internal team.

| Role | Capabilities |
|---|---|
| Superadmin | Full access across every module, including user management and deletions |
| Admin | Manages most modules; user management is limited to creating accounts |
| Marketing | Manages orders and subscriptions |
| Finance | Manages payments, bills, and invoices; read-only on clients and products |
| Client | Sees only its own bills and orders |
| Viewer | Read-only across every module; all action buttons are hidden |

---

## ≡ƒöÆ Security

Security best practices are applied throughout the platform ΓÇö from secure session management and access control on every endpoint, to safe file handling and hardened web headers.

---

## ≡ƒôä License

This project is licensed under the MIT License ΓÇö see the [LICENSE](LICENSE) file for details.

---

## ≡ƒæñ Author

**Melvin** ([@CodeMelvin](https://github.com/CodeMelvin))
