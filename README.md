# Free UI Templates

Free, customizable templates for websites, dashboards, admin panels, and full-stack learning projects. This repo is a **catalog hub** for the [Poluru Labs](https://github.com/poluru-labs) open-source collections below. Clone any linked repository, pick a template or project folder, and run it locally.

---

## Collections at a glance

| Collection | Stack | Best for |
| --- | --- | --- |
| [Enterprise Web Components Templates](#enterprise-web-components-templates) | Vite, vanilla custom elements, Bootstrap 5, `@poluru-labs/enterprise-design-system-wc` | Framework-agnostic enterprise dashboards with reusable `eds-*` controls |
| [Enterprise Vue Free AI Web Templates](#enterprise-vue-free-ai-web-templates) | Vue 3, Vite, Vue Router, `@poluru-labs/enterprise-design-system-vue` | AI SaaS, CRM, HR, finance, and ops dashboards |
| [Enterprise React Free AI Web Templates](#enterprise-react-free-ai-web-templates) | React 18+, Vite, React Router, `@poluru-labs/enterprise-design-system-react` | AI ops consoles, LLM ops, RAG, moderation, and admin workspaces |
| [Enterprise Angular Free AI Web Templates](#enterprise-angular-free-ai-web-templates) | Angular 21, standalone components, `@poluru-labs/enterprise-design-system-angular` | 35 AI-focused admin and ops demos with signals + OnPush |
| [Free Web & Mobile Templates](#subrahmanyam-poluru-free-web--mobile-templates) | HTML, Bootstrap 5, Chart.js (no build step) | Marketing sites, admin dashboards, and vertical landing pages |
| [FastAPI Real-World Projects](#fastapi-realworld-projects) | Python, FastAPI, Docker, tests | Backend APIs with auth, databases, WebSockets, and jobs |
| [PHPKingdom Tutorials](#phpkingdom) | HTML examples, Node.js tracks, local catalog dashboard | Large tutorial library with exercises and starter templates |

---

## Enterprise Web Components Templates

**Repository:** [github.com/poluru-labs/enterprise-web-components-templates](https://github.com/poluru-labs/enterprise-web-components-templates)

Free enterprise-grade dashboard and web app templates built with **Bootstrap 5**, **Bootstrap Icons**, **Vite**, and **`@poluru-labs/enterprise-design-system-wc`**. Each template is a standalone Vite app with its own `package.json`, mock data, hash-based routing (including search), Vitest tests, and publishable package manifest.

**Highlights**

- Vanilla **custom elements** for shell, header, sidebar, and equal-height content cards
- **`eds-*`** design-system tags for forms, tables, drawers, and toasts
- Distinct header chrome per product (tickers, pipeline pills, SLA ribbons, and similar)
- **Node.js 20+** required; no root monorepo `package.json`—work inside one template folder

**Featured templates (19 workflows)**

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

**Getting started**

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

---

## Enterprise Vue Free AI Web Templates

**Repository:** [github.com/poluru-labs/enterprise-vue-free-ai-web-templates](https://github.com/poluru-labs/enterprise-vue-free-ai-web-templates)

A curated collection of **Vue 3** templates for AI dashboards, SaaS products, admin panels, and internal tools. Each app is a self-contained **Vite** project using **`@poluru-labs/enterprise-design-system-vue`**, **Vue Router**, **Bootstrap 5**, **Bootstrap Icons**, and **Vitest**.

**Templates**

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

**Getting started** (Node.js 20+)

```bash
git clone https://github.com/poluru-labs/enterprise-vue-free-ai-web-templates.git
cd enterprise-vue-free-ai-web-templates/ai-admin-dashboard
npm install
npm run dev
```

Typical layout: `src/components/layout/` (AppShell, AppHeader, AppSidebar), `components/widgets/`, `views/`, `router/`, `stores/`, and `data/`.

---

## Enterprise React Free AI Web Templates

**Repository:** [github.com/poluru-labs/enterprise-react-free-ai-web-templates](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates)

Production-shaped **React** templates for AI dashboards, ops consoles, and admin workspaces. Each folder is an independent **Vite** app with **`@poluru-labs/enterprise-design-system-react`**, **Bootstrap 5**, mock data under `src/data/`, and **Vitest** where included. **MIT** license.

**Templates**

| Folder | Product | Focus |
| --- | --- | --- |
| `ai-agent-monitoring-dashboard` | AgentPulse | Fleet ops, incidents, traces, guardrails, cost |
| `ai-computer-vision-dashboard` | Sightline | Cameras, models, detections, quality |
| `ai-content-moderation-dashboard` | ReviewBay | Queue, policies, appeals, automation |
| `ai-data-pipeline-dashboard` | Conduit | Ingestion, transformations, lineage |
| `ai-marketing-command-center` | Marquee | Campaigns, audiences, content |
| `ai-document-rag-dashboard` | Contextly | Ingestion, retrieval, citations, evals |
| `ai-governance-compliance-dashboard` | Charter | Inventories, risk, policies, approvals |
| `ai-llm-ops-dashboard` | Poluru LLM Ops | Traces, playground, evals, cost |
| `ai-ml-training-dashboard` | Kiln | Training runs, datasets, GPU clusters |
| `ai-model-evaluation-dashboard` | Prism | Eval suites, leaderboards, human review |
| `ai-prompt-management-dashboard` | Prompt Bureau | Library, versions, evals, releases |
| `ai-saas-admin-dashboard` | Nexus | Tenants, billing, flags, audit |
| `ai-support-helpdesk-dashboard` | Relay | Inbox, SLA, macros, copilot drafts |
| `ai-synthetic-data-studio` | Poluru Synth Studio | Synthetic data, privacy, TSTR evals |
| `enterprise-dashboard` | Poluru DC | Facilities, power, capacity, tickets (React 19 + TS) |

Additional folders in the repo include agent builder, API gateway, document processing, edge inference, energy optimization, experimentation, financial risk, and related AI ops surfaces. Some entries (for example voice operations and security operations) may be README stubs until the Vite app lands—check each folder before running.

**Getting started** (Node.js 20+; Node 18 works on several older templates)

```bash
git clone https://github.com/poluru-labs/enterprise-react-free-ai-web-templates.git
cd enterprise-react-free-ai-web-templates/ai-agent-monitoring-dashboard
npm install
npm run dev
```

| Script | Description |
| --- | --- |
| `npm run dev` | Vite development server |
| `npm test` | Vitest + Testing Library (where present) |
| `npm run build` | Production build |
| `npm run preview` | Preview production build |

---

## Enterprise Angular Free AI Web Templates

**Repository:** [github.com/poluru-labs/enterprise-angular-free-ai-web-templates](https://github.com/poluru-labs/enterprise-angular-free-ai-web-templates)

**35** standalone **Angular 21** demos for AI dashboards, ops consoles, and admin workspaces. Uses **`@poluru-labs/enterprise-design-system-angular`**, light UI with per-template brand colors, **Roboto + Lato** on EDS dashboards, demo data, **signals + `OnPush`** on showcase apps, and **`ng build`** / **`ng test --watch=false`** in each project. **MIT** license.

**Sample of templates**

| Folder | Title | Focus |
| --- | --- | --- |
| `ai-agent-marketplace-admin` | Agent Marketplace Admin | Listings, approvals, pricing |
| `ai-agent-ops-console` | AgentOps Kit | Fleet health, runs, tools, deploys |
| `ai-prompt-playground` | Prompt Playground | Multi-model prompt test, variables, diff |
| `ai-rag-knowledge-admin` | Indigo Vault | RAG sources, indexing, retrieval |
| `ai-llm-usage-dashboard` | Lilac Meter | Token spend, latency, budgets |
| `ai-red-teaming-console` | Red Teaming Console | Attack suites, findings, severity |
| `ai-workflow-orchestration-ui` | Workflow Orchestration | Pipeline builder, runs, HITL |
| `ai-support-copilot-dashboard` | Harbor Desk | Support queue, drafts, CSAT |
| `ai-guardrails-policy-center` | Reef · Guardrails | Filters, PII, safety policies |

See the [full 35-template table](https://github.com/poluru-labs/enterprise-angular-free-ai-web-templates#templates-35) in the upstream README.

**Getting started** (Node.js 20+ LTS)

```bash
git clone https://github.com/poluru-labs/enterprise-angular-free-ai-web-templates.git
cd enterprise-angular-free-ai-web-templates/ai-prompt-playground
npm install
npm start
```

Default URL: `http://localhost:4200/`. Run multiple demos with `ng serve --port 4215` (or another free port).

Customize brand tokens in `src/styles.scss`, shell and demo data in `src/app/app.ts` / `app.html`, and router apps under `src/app/features/…`.

---

## Subrahmanyam Poluru Free Web & Mobile Templates

**Repository:** [github.com/poluru-labs/subrahmanyam-poluru-free-web-mobile-templates](https://github.com/poluru-labs/subrahmanyam-poluru-free-web-mobile-templates)

Responsive **Bootstrap 5** website and admin templates—**no build step**. Templates live under `web/bootstrap/` with HTML, assets, and per-template README files. Browse all entries from [`web/bootstrap/index.html`](https://github.com/poluru-labs/subrahmanyam-poluru-free-web-mobile-templates/tree/main/web/bootstrap).

**Available templates**

| # | Name | Location | Notes |
| ---: | --- | --- | --- |
| 1 | IT Consulting | `web/bootstrap/it-consulting` | Multi-page consulting site |
| 2 | Teams Chat | `web/bootstrap/teams-chat` | Chat UI with sidebar and demo behavior |
| 3 | Web Design | `web/bootstrap/webdesign` | Agency landing page |
| 4 | Modern Admin Dashboard | `web/bootstrap/modern-admin-dashboard` | Ecommerce admin, KPIs, charts |
| 5 | Modern Admin Network Dashboard | `web/bootstrap/modern-admin-network-dashboard` | 11-page SecOps platform |
| 6 | Nonprofit Impact Dashboard | `web/bootstrap/non-profit-impact-dashboard` | Public impact site, donate CTA |
| 7 | Elevate Awards | `web/bootstrap/elevate-awards` | Nomination and judging workflow |
| 8 | Founder Metrics Dashboard | `web/bootstrap/founder-metrics-dashboard-app` | Investor-ready KPI board |
| 9 | Researcher Portfolio | `web/bootstrap/researcher-portfolio` | Academic portfolio (AOS animations) |
| 10 | Startup KPI Board | `web/bootstrap/startup-kpi-board` | MRR, ARR, CAC, LTV, runway |
| 11 | Restaurant Reservation | `web/bootstrap/restaurant-reservation` | Menu, booking, events |
| 12 | Hotel Booking | `web/bootstrap/hotel-booking` | Rooms, amenities, reservations |
| 13 | Real Estate Platform | `web/bootstrap/real-estate-platform` | Listings, agents, inquiries |
| 14 | Travel Tour Agency | `web/bootstrap/travel-tour-agency` | Tours, packages, itineraries |

**Technologies:** HTML5, CSS3, Bootstrap 5, JavaScript, Bootstrap Icons, Google Fonts (Inter), Chart.js on admin templates.

**Getting started**

```bash
git clone https://github.com/poluru-labs/subrahmanyam-poluru-free-web-mobile-templates.git
cd subrahmanyam-poluru-free-web-mobile-templates/web/bootstrap/modern-admin-network-dashboard
python3 -m http.server 8000
# Open http://localhost:8000
```

**Author:** [Subrahmanyam Poluru](https://polurus.com) · mail.polurus@gmail.com

---

## fastapi-realworld-projects

**Repository:** [github.com/poluru-labs/fastapi-realworld-projects](https://github.com/poluru-labs/fastapi-realworld-projects)

Real-world **FastAPI** projects with **authentication**, **databases**, **WebSockets**, and **background jobs**. Includes **tests**, **Docker** setup, and step-by-step guides. **MIT** license.

**Structure**

| Track | Folder | Purpose |
| --- | --- | --- |
| Beginner | `beginner/` | Foundational APIs and patterns |
| Intermediate | `intermediate/` | Auth, persistence, and common production patterns |
| Advanced | `advanced/` | WebSockets, jobs, and richer architectures |

Clone the repo and open the README inside each track or project folder for run instructions, environment variables, and Docker commands.

```bash
git clone https://github.com/poluru-labs/fastapi-realworld-projects.git
cd fastapi-realworld-projects
# Follow README in beginner/, intermediate/, or advanced/
```

---

## PHPKingdom

**Repository:** [github.com/poluru-labs/phpkingdom](https://github.com/poluru-labs/phpkingdom)

Tutorial packs for **[phpkingdom.com](https://phpkingdom.com)**—practical HTML examples, exercises, and starter templates for web and Node.js topics. Includes a local **Bootstrap 5 dashboard** (brand **PHPKINGDOM** `#DA0037`) to browse courses and open examples.

**Scale (approximate)**

| Metric | Count |
| --- | ---: |
| Courses | 35 |
| Topics | 3,862 |
| Examples | 85,907 |
| Exercises | 1,325 |
| Templates | 875 |

**Course tracks** include Angular, React, Vue, Next.js, NestJS, Node.js, Express, GraphQL, DynamoDB, Kafka, AWS Lambda, Authentication, Design Systems, Web Components, Lit, Cypress, Playwright, Jest, Git, HTML/CSS, TypeScript, Tailwind, Webpack, Module Federation, Single-SPA, Web Accessibility, UI libraries, and more.

**Local dashboard**

```bash
git clone https://github.com/poluru-labs/phpkingdom.git
cd phpkingdom
npm install
npm run generate   # builds data/catalog.json + data/courses/*.json
npm run dev        # http://localhost:4173
```

Lessons use sibling `.css` / `.js` files next to `.html` pages; CDNs remain for Bootstrap, Tailwind Play, Lit, and similar where lessons require them.

**Author:** Subrahmanyam Poluru · mail.polurus@gmail.com · [polurus.com](https://polurus.com)

---

## Shared design system

Several enterprise template repos depend on Poluru Labs npm packages:

| Framework | Package |
| --- | --- |
| Web Components | `@poluru-labs/enterprise-design-system-wc` |
| Vue | `@poluru-labs/enterprise-design-system-vue` |
| React | `@poluru-labs/enterprise-design-system-react` |
| Angular | `@poluru-labs/enterprise-design-system-angular` |

Install dependencies inside each template’s folder; versions are pinned per app `package.json`.

---

## Contributing

Explore, fork, and open pull requests on the individual repositories linked above. Improvements to this catalog README are welcome in **free-ui-templates**.

## License

Licensing varies by repository (for example **MIT** on several Poluru Labs template repos). Check each linked repo’s `LICENSE` file before redistribution.
