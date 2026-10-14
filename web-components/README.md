# Enterprise Web Components Templates

**Repository:** [github.com/poluru-labs/enterprise-web-components-templates](https://github.com/poluru-labs/enterprise-web-components-templates)

Free enterprise-grade dashboard and web app templates built with **Bootstrap 5**, **Bootstrap Icons**, **Vite**, and **`@poluru-labs/enterprise-design-system-wc`**. Each template is a standalone Vite app with its own `package.json`, mock data, hash-based routing (including search), Vitest tests, and publishable package manifest.

Part of the [Free UI Templates](../README.md) catalog.

## Highlights

- Vanilla **custom elements** for shell, header, sidebar, and equal-height content cards
- **`eds-*`** design-system tags for forms, tables, drawers, and toasts
- Distinct header chrome per product (tickers, pipeline pills, SLA ribbons, and similar)
- **Node.js 20+** required; no root monorepo `package.json`—work inside one template folder

## Featured templates (19 workflows)

| Product | Use case | Dev port | Folder |
| --- | --- | ---: | --- |
| Signal | Executive KPIs and scorecards | 5178 | `enterprise-kpi-dashboard` |
| Lyra | Pipeline, accounts, and deals | 5179 | `enterprise-crm-dashboard` |
| Alder | People, leave, hiring, learning | 5181 | `enterprise-hrms-portal` |
| Vespera | Projects, sprints, and capacity | 5177 | `enterprise-project-dashboard` |
| Verdant | Invoices, AR, and subscriptions | 5174 | `enterprise-billing-dashboard` |
| Nimbus | Stock, inbound, and warehouses | 5183 | `enterprise-inventory-dashboard` |
| Halo | Appointments, patients, census | 5175 | `enterprise-clinic-admin` |
| Relay | Tickets, SLA, and queues | 5180 | `enterprise-helpdesk-portal` |
| Helix | Reports, quality, and insights | 5173 | `enterprise-bi-dashboard` |
| Helio | Orgs, seats, and uptime | 5176 | `enterprise-saas-admin` |
| Atlas | Procurement, suppliers, spend | 5184 | `enterprise-procurement-portal` |
| Aegis | Policies, controls, audit readiness | 5185 | `enterprise-compliance-dashboard` |
| Sentinel | Security operations and incidents | 5186 | `enterprise-security-operations` |
| Orbit | Fleet, maintenance, drivers | 5187 | `enterprise-fleet-management` |
| Keystone | Construction sites, RFIs, safety | 5188 | `enterprise-construction-dashboard` |
| Haven | Real estate, leases, occupancy | 5189 | `enterprise-real-estate-portal` |
| Beacon | Insurance claims and settlements | 5190 | `enterprise-insurance-claims` |
| Aurevia | Banking payments and clearing | 5191 | `enterprise-banking-operations` |
| Loom | Content operations and publishing | 5192 | `enterprise-content-operations` |

The repo also includes additional enterprise folders (for example customer success, data governance, developer platform, education, energy, events, hospitality, logistics, manufacturing, marketing, public sector, revenue cycle, subscriptions, travel, and vendor management). Browse the full tree on GitHub.

## Getting started

```bash
git clone https://github.com/poluru-labs/enterprise-web-components-templates.git
cd enterprise-web-components-templates/enterprise-bi-dashboard   # any template folder
npm install
npm run dev
```

| Script | Purpose |
| --- | --- |
| `npm run dev` | Local development server |
| `npm test` | Vitest + jsdom unit tests |
| `npm run build` | Production build (`base: './'`) |
| `npm run preview` | Preview production build |

Use **Cmd+K** / **Ctrl+K** for command navigation; header search opens `#/search`.

## Design system

Install dependencies inside each template folder. The Web Components package is **`@poluru-labs/enterprise-design-system-wc`**, pinned in that app’s `package.json`.

## License

Check the upstream `LICENSE` before redistribution.
