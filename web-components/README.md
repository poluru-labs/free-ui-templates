# Enterprise Web Components Templates

**Repository:** [github.com/poluru-labs/enterprise-web-components-templates](https://github.com/poluru-labs/enterprise-web-components-templates)

Free enterprise-grade dashboard and web app templates built with **Bootstrap 5**, **Bootstrap Icons**, **Vite**, and **`@poluru-labs/enterprise-design-system-wc`**. Each template is a standalone Vite app with its own `package.json`, mock data, hash-based routing (including search), Vitest tests, and publishable package manifest.

Part of the [Free UI Templates](../README.md) catalog.

## Highlights

- Vanilla **custom elements** for shell, header, sidebar, and equal-height content cards
- **`eds-*`** design-system tags for forms, tables, drawers, and toasts
- Distinct header chrome per product (tickers, pipeline pills, SLA ribbons, and similar)
- **Node.js 20+** required; no root monorepo `package.json`—work inside one template folder

## Available templates

**50** Vite applications (folder names are at the repository root). Dev **port** comes from each app’s `vite.config.js`—several apps share **5178**; change `server.port` if you run more than one at a time.

### AI & quality workspaces

| Product | Use case | Port | Folder |
| --- | --- | ---: | --- |
| Beacon | Accessibility audit workspace | 5178 | `enterprise-ai-accessibility-auditor` |
| Relay | AI agent / workflow run observability | 5184 | `enterprise-ai-agent-observability` |
| Bench | Component testing lab | 5179 | `enterprise-ai-component-testing-lab` |
| Probe | Dataset quality inspection | 5187 | `enterprise-ai-dataset-quality-inspector` |
| Atelier | Design system workbench | 5180 | `enterprise-ai-design-system-workbench` |
| Clarity | Document accessibility review | 5181 | `enterprise-ai-document-accessibility` |
| Panel | Human review workspace | 5188 | `enterprise-ai-human-review-workspace` |
| Gauge | Inference benchmarking & SLO tracking | 5190 | `enterprise-ai-inference-benchmarking` |
| Gauge | Model evaluation workspace | 5182 | `enterprise-ai-model-evaluation` |
| Lexicon | Multilingual knowledge search | 5186 | `enterprise-ai-multilingual-knowledge-search` |
| Beacon | Open source impact tracking | 5191 | `enterprise-ai-open-source-impact-tracker` |
| Seal | Prompt / input security testing | 5189 | `enterprise-ai-prompt-security-testing` |
| Anchor | RAG & retrieval quality analyzer | 5183 | `enterprise-ai-rag-quality-analyzer` |
| Ledger | Research reproducibility | 5185 | `enterprise-ai-research-reproducibility` |

### Core enterprise workflows

| Product | Use case | Port | Folder |
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

### Extended operations & industry

| Product | Use case | Port | Folder |
| --- | --- | ---: | --- |
| Vista | Hospitality claims & guest operations copilot | 5178 | `enterprise-claims-copilot` |
| Pulse | Customer success, health, renewals | 5182 | `enterprise-customer-success` |
| Verity | Data catalog, lineage, governance | 5178 | `enterprise-data-governance` |
| Circuit | Developer platform & deployments | 5186 | `enterprise-developer-platform` |
| Signal | Education administration | 5178 | `enterprise-education-admin` |
| Terra | Energy production & sustainability ops | 5178 | `enterprise-energy-operations` |
| Gather | Event registrations & venues | 5185 | `enterprise-event-management` |
| Signal | Hospitality management | 5178 | `enterprise-hospitality-management` |
| TechStar | IT assets, incidents, change | 5188 | `enterprise-it-operations` |
| Meridian | Logistics control tower | 5178 | `enterprise-logistics-control-tower` |
| Signal | Manufacturing operations | 5178 | `enterprise-manufacturing-dashboard` |
| Signal | Marketing operations | 5178 | `enterprise-marketing-operations` |
| CivicWorks | Public sector permits & cases | 5184 | `enterprise-public-sector-portal` |
| Signal | Revenue cycle & billing ops | 5178 | `enterprise-revenue-cycle-dashboard` |
| Prism | Subscription lifecycle management | 5178 | `enterprise-subscription-management` |
| Waypoint | Travel trips, approvals, itineraries | 5183 | `enterprise-travel-operations` |
| Harbor | Vendor onboarding, risk, contracts | 5178 | `enterprise-vendor-management` |

Per-template README files and package `description` fields in the upstream repo have brand colors and header chrome details.

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

## Author

[Subrahmanyam Poluru](https://polurus.com) · mail.polurus@gmail.com
