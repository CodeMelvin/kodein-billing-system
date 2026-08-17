# Kodein Billing System

A billing, subscription, and invoicing platform built during my time at Kodein, an Indonesian IT company based in Jakarta.

## Screenshots

| Login | Dashboard | Billing |
|---|---|---|
| <img src="screenshots/login.png" width="220"/> | <img src="screenshots/dashboard.png" width="220"/> | <img src="screenshots/billing.png" width="220"/> |

| Orders | Subscriptions | Products |
|---|---|---|
| <img src="screenshots/orders.png" width="220"/> | <img src="screenshots/subscriptions.png" width="220"/> | <img src="screenshots/products.png" width="220"/> |

Screenshots are also available in the [`screenshots/`](screenshots/) folder.

## What this is

Kodein Billing System replaces a spreadsheet-based workflow with a single dashboard for managing the full lifecycle of a client project: order approval, progress tracking, recurring subscriptions, and invoicing. The team can see what is in progress, what needs approval, and what is due for payment without asking around.

This is a demo build. All data shown is sample data for illustration only.

## Why it was built

Kodein designs, develops, and hosts websites and mobile applications for businesses across Indonesia. With several projects running at once, tracking down payments, deadlines, and recurring hosting fees became a job of its own. This platform gives the team one place to keep that under control. You can see examples of Kodein's work on their [portfolio](https://kodein.co.id/portofolio).

## Features

- Project management with configurable down payments, progress milestones, and file attachments
- Recurring subscriptions with weekly, monthly, and annual billing periods, plus a grace period, suspension, and re-billing lifecycle
- Automatic bill generation, invoice and proof-of-payment uploads, approve, decline, and refund workflows, with tax support
- Invoice PDF generation on demand
- In-app notifications for approvals, renewals, and expiring bills
- Role-based access for admins, finance, marketing, clients, and a read-only viewer

## Built with

- Next.js (App Router), React, TypeScript
- Tailwind CSS
- PostgreSQL
- JWT session handling with rotating refresh tokens
- Vercel for hosting and scheduled jobs

## Live demo

The live demo runs at [https://kodein-billing-system.vercel.app](https://kodein-billing-system.vercel.app).

One account is open for public testing, and it is read-only:

| Role | Email | Password |
|---|---|---|
| Viewer | `viewer.demo.BTp2@example.com` | `PWzvj6-DH9QxG-7PP7mc` |

The viewer can browse every module but cannot create, edit, delete, approve, or upload anything. The other roles listed below are not available for public login.

## Roles

The system supports five roles besides the viewer, each with its own scope. Credentials for these roles are deliberately not published; they belong to the internal team.

| Role | Can do |
|---|---|
| Superadmin | Full access across every module, including user management and deletions |
| Admin | Manages most modules; user management is limited to creating accounts |
| Marketing | Manages orders and subscriptions |
| Finance | Manages payments, bills, and invoices; read-only on clients and products |
| Client | Sees only its own bills and orders |
| Viewer | Read-only across every module; all action buttons are hidden |

## Security

The codebase applies standard web security practices: bcrypt password hashing, httpOnly secure session cookies, rate limiting on authentication endpoints, parameterized SQL queries, validated file uploads, and access checks on every API route. No real data is stored; all records in the demo are fictitious.

## License

MIT. See the [LICENSE](LICENSE) file.

## Author

Melvin ([@CodeMelvin](https://github.com/CodeMelvin))