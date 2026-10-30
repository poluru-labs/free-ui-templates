# Enterprise React Free AI Web Templates

**Repository:** [github.com/poluru-labs/enterprise-react-free-ai-web-templates](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates)

Production-shaped **React** templates for AI dashboards, ops consoles, and admin workspaces. **36** folders — **35** are independent **Vite** apps with **`@poluru-labs/enterprise-design-system-react`**, mock data under `src/data/`, and **Vitest** where included. **MIT** license.

Part of the [Free UI Templates](../README.md) catalog.

## Featured templates

| Folder | Product | Focus | Dev port |
| --- | --- | --- | ---: |
| `ai-agent-monitoring-dashboard` | AgentPulse | Fleet ops, incidents, traces, guardrails, cost | 5173 |
| `ai-computer-vision-dashboard` | Sightline | Cameras, models, detections, quality | 5173 |
| `ai-content-moderation-dashboard` | ReviewBay | Queue, policies, appeals, automation | 5173 |
| `ai-data-pipeline-dashboard` | Conduit | Ingestion, transformations, lineage | 5192 |
| `ai-marketing-command-center` | Marquee | Campaigns, audiences, content | 5193 |
| `ai-document-rag-dashboard` | Contextly | Ingestion, retrieval, citations, evals | 5173 |
| `ai-governance-compliance-dashboard` | Charter | Inventories, risk, policies, approvals | 5191 |
| `ai-llm-ops-dashboard` | Poluru LLM Ops | Traces, playground, evals, cost | 5185 |
| `ai-ml-training-dashboard` | Kiln | Training runs, datasets, GPU clusters | 5184 |
| `ai-model-evaluation-dashboard` | Prism | Eval suites, leaderboards, human review | 5186 |
| `ai-prompt-management-dashboard` | Prompt Bureau | Library, versions, evals, releases | 5187 |
| `ai-saas-admin-dashboard` | Nexus | Tenants, billing, flags, audit | 5188 |
| `ai-support-helpdesk-dashboard` | Relay | Inbox, SLA, macros, copilot drafts | 5189 |
| `ai-synthetic-data-studio` | Poluru Synth Studio | Synthetic data, privacy, TSTR evals | 5194 |
| `enterprise-dashboard` | Poluru DC | Facilities, power, capacity, tickets (React 19 + TS) | 5173 |

Several apps share Vite’s default **5173** — start those one at a time, or pass `--port` to `npm run dev`. Prism uses hash routes (`#/overview`).

## All template folders

| Folder | Product / title | Status |
| --- | --- | --- |
| `ai-agent-builder-studio` | Agent Builder Studio | App |
| `ai-agent-monitoring-dashboard` | AgentPulse | App |
| `ai-api-gateway-dashboard` | API Gateway (starter shell) | App |
| `ai-computer-vision-dashboard` | Sightline | App |
| `ai-content-moderation-dashboard` | ReviewBay | App |
| `ai-data-pipeline-dashboard` | Conduit | App |
| `ai-document-processing-dashboard` | Pagewise | App |
| `ai-document-rag-dashboard` | Contextly | App |
| `ai-edge-inference-dashboard` | CareLine / edge inference | App |
| `ai-energy-optimization-dashboard` | GridPulse | App |
| `ai-experimentation-platform` | VariantLab | App |
| `ai-financial-risk-dashboard` | RiskPulse | App |
| `ai-forecasting-planning-dashboard` | PlanPulse | App |
| `ai-governance-compliance-dashboard` | Charter | App |
| `ai-healthcare-operations-dashboard` | ClinicPulse | App |
| `ai-human-in-the-loop-workspace` | ReviewLoop | App |
| `ai-knowledge-base-dashboard` | KnowPulse | App |
| `ai-legal-contract-intelligence-dashboard` | ContractPulse | App |
| `ai-llm-ops-dashboard` | Poluru LLM Ops | App |
| `ai-marketing-command-center` | Marquee | App |
| `ai-marketing-intelligence-dashboard` | Marketing Intelligence | App |
| `ai-ml-training-dashboard` | Kiln | App |
| `ai-model-evaluation-dashboard` | Prism | App |
| `ai-personalization-dashboard` | Personalization | App |
| `ai-prompt-management-dashboard` | Prompt Bureau | App |
| `ai-recommendation-engine-dashboard` | Recommendation Engine | App |
| `ai-robotics-fleet-dashboard` | Robotics Fleet | App |
| `ai-saas-admin-dashboard` | Nexus | App |
| `ai-search-analytics-dashboard` | Search Analytics (starter shell) | App |
| `ai-security-operations-center` | Security Operations | README stub only |
| `ai-supply-chain-control-tower` | Supply Chain Control Tower | App |
| `ai-support-helpdesk-dashboard` | Relay | App |
| `ai-synthetic-data-studio` | Poluru Synth Studio | App |
| `ai-translation-operations-dashboard` | Translation Operations | App |
| `ai-voice-operations-dashboard` | Voice Operations | App |
| `enterprise-dashboard` | Poluru DC | App |

Browse any folder on GitHub:

`https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/tree/main/<folder-name>`

## Getting started

Node.js 20+ (Node 18 works on several older templates).

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

Each template has its own `package.json` — install and run inside that folder only.

## Stack

Most templates share:

- React 18 + React Router 6 (**Poluru DC** uses React 19, Router 7, and TypeScript)
- Vite
- Bootstrap 5 + Bootstrap Icons (**Poluru DC** uses SCSS instead of Bootstrap)
- [`@poluru-labs/enterprise-design-system-react`](https://www.npmjs.com/package/@poluru-labs/enterprise-design-system-react)
- Vitest + Testing Library + jsdom

Typical layout:

```text
src/
  App.jsx (or App.tsx)
  main.jsx
  components/layout/     header, sidebar, shell
  components/widgets/    page header, stat cards, tables
  components/charts/     SVG sparklines and charts
  data/                  JSON fixtures
  pages/ or views/
  test/setup.js
```

Copy and mock data live in `src/data/`. Brand color and shell chrome live in each app’s CSS/SCSS and layout components.

## Design system

Install dependencies inside each template folder. The React package is **`@poluru-labs/enterprise-design-system-react`**, pinned in that app’s `package.json`.

Source: [enterprise-design-system-react](https://github.com/poluru-labs/enterprise-design-system-react) · npm: [@poluru-labs/enterprise-design-system-react](https://www.npmjs.com/package/@poluru-labs/enterprise-design-system-react)

## License

**MIT** on this collection. Check the upstream `LICENSE` before redistribution.
