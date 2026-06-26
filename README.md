# Quenta ERP — Full-Stack ERP System

A multi-tenant SaaS ERP platform built for Philippine SMEs. Designed and coded solo under JD Solutions Ph.

Deployed and actively being developed — some modules are production-ready, others still being finished.

**Live:** https://quenta-erp.vercel.app
![ERP Dashboard Screenshot](dashboard.png)

---

## What It Does

Quenta ERP covers the core operations of a small-to-medium business:

- **POS** — sales transactions, receipt printing, Z-reading, session close with auto journal posting
- **Inventory** — stock management, supplier tracking, purchase receiving with inventory deduction
- **Payroll** — BIR TRAIN Law withholding, SSS/PhilHealth/Pag-IBIG, DTR, payslip generation
- **Accounting** — Chart of Accounts, journal entries, general ledger, financial reports (Income Statement, Balance Sheet, Cash Flow, AR/AP Aging)
- **BIR Compliance** — SAWT, QAP, SLSP, MAP report generation
- **AI Business Assistant** — Anthropic API + custom MCP server, business owners can query their own data in natural language (finishing production testing)
- **PWA Modules** — PostWatch (security guard management), Pandesal Rider (delivery tracking), Grocery POS
- **Marketplace Hub** — multi-channel product publishing (in development)

---

## Tech Stack

**Frontend**
- Next.js 14
- React
- Tailwind CSS
- TypeScript

**Backend**
- Node.js (Next.js API routes)
- PostgreSQL (hosted on Supabase)
- 20+ schemas, multi-tenant architecture

**Infrastructure**
- Supabase (database, auth, storage)
- Vercel (hosting, serverless)
- n8n (automation workflows)

---

## Architecture Highlights

- Multi-tenant from day one — every query filters by `tenant_id` and `company_id` from server-side session
- 20+ PostgreSQL schemas — one per ERP module
- Server-side session only — `tenant_id` and `company_id` never come from client
- Double-entry accounting engine — all financial transactions post to general ledger
- PWA-ready modules — service worker, offline support, installable on mobile
- AI layer — Anthropic Messages API with function calling, custom MCP server

---

## My Role

Designed and built everything:
- System architecture and database schema design
- All frontend interfaces and components
- All backend API routes (40+)
- PostgreSQL query logic and reporting
- Multi-tenant session and security layer
- PWA service workers and manifests
- n8n automation workflows
- AI Business Assistant architecture

---

## GitHub

[bqygithub](https://github.com/bqygithub)
