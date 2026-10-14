# Enterprise Vue Free AI Web Templates

**Repository:** [github.com/poluru-labs/enterprise-vue-free-ai-web-templates](https://github.com/poluru-labs/enterprise-vue-free-ai-web-templates)

A curated collection of **Vue 3** templates for AI dashboards, SaaS products, admin panels, and internal tools. Each app is a self-contained **Vite** project using **`@poluru-labs/enterprise-design-system-vue`**, **Vue Router**, **Bootstrap 5**, **Bootstrap Icons**, and **Vitest**.

Part of the [Free UI Templates](../README.md) catalog.

## Templates

| Template | Description | Dev port |
| --- | --- | ---: |
| Harbor Admin (`ai-admin-dashboard`) | Tenants, seats, flags, audit — theme `#0F172A` | 5190 |
| Bloom CRM (`ai-crm-template`) | Pipeline, accounts, sales activity — `#F13E93` | 5191 |
| Pulse Analytics (`ai-saas-analytics-dashboard`) | Activation, retention, usage — `#4F46E5` | 5192 |
| Lumen Helpdesk (`ai-helpdesk-support-portal`) | Queues, SLAs, suggested replies — `#0284C7` | 5193 |
| Grove HR (`ai-hr-management-dashboard`) | Headcount, leave, hiring, learning — `#7C3AED` | 5194 |
| Keel Projects (`ai-project-management-app`) | Boards, sprints, delivery risk — `#0F766E` | 5195 |
| Mint Finance (`ai-finance-expense-dashboard`) | Spend, invoices, month-end close — `#047857` | 5196 |
| Vault Documents (`ai-document-workspace`) | Library, reviews, search — `#B45309` | 5197 |
| Quota Sales Ops (`ai-sales-ops-dashboard`) | Forecast, coverage, hygiene — `#1E3A8A` | 5198 |
| Atlas Intranet (`ai-knowledge-base-intranet-template`) | Spaces, how-tos, policies — `#3F6212` | 5199 |
| Aegis Compliance (`ai-compliance-management-dashboard`) | Controls, audits, risks — `#FF5722` | 5200 |
| Folio Content Ops (`ai-content-operations-platform`) | Plan, create, review, publish — `#102E50` | 5201 |
| Marigold Success (`ai-customer-success-hub`) | Health, renewals, onboarding — `#F2C46A` | 5202 |
| Cobalt Governance (`ai-data-governance-platform`) | Ownership, quality, catalogs — `#3368A0` | 5203 |

## Getting started

Node.js 20+.

```bash
git clone https://github.com/poluru-labs/enterprise-vue-free-ai-web-templates.git
cd enterprise-vue-free-ai-web-templates/ai-admin-dashboard
npm install
npm run dev
```

Typical layout: `src/components/layout/` (AppShell, AppHeader, AppSidebar), `components/widgets/`, `views/`, `router/`, `stores/`, and `data/`.

## Design system

Install dependencies inside each template folder. The Vue package is **`@poluru-labs/enterprise-design-system-vue`**, pinned in that app’s `package.json`.

## License

Check the upstream `LICENSE` before redistribution.
