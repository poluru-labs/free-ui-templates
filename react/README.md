# Enterprise React Free AI Web Templates

**Repository:** [github.com/poluru-labs/enterprise-react-free-ai-web-templates](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates)

Free, production-shaped **React** templates for AI dashboards, ops consoles, and admin workspaces. **49** template folders — **48** are self-contained **Vite** apps with **Bootstrap 5**, [`@poluru-labs/enterprise-design-system-react`](https://www.npmjs.com/package/@poluru-labs/enterprise-design-system-react), mock data under `src/data/`, and **Vitest** where included. Maintained by [Poluru Labs](https://polurus.com). **MIT** license.

Part of the [Free UI Templates](../README.md) catalog.

Clone the upstream repo, `cd` into any folder below, then `npm install` and `npm run dev`.

## Showcase templates

Curated apps with product names, brand colors, and typical local entry URLs (after `npm run dev` in that folder):

| Template | Product | What it covers | Brand | Local demo |
| --- | --- | --- | --- | --- |
| [Agent monitoring](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-agent-monitoring-dashboard/README.md) | AgentPulse | Fleet ops, incidents, traces, guardrails, and cost | `#003161` | [localhost:5173/agent-monitoring/overview](http://localhost:5173/agent-monitoring/overview) |
| [Computer vision](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-computer-vision-dashboard/README.md) | Sightline | Cameras, models, detections, and quality | `#0F766E` | [localhost:5173/computer-vision/overview](http://localhost:5173/computer-vision/overview) |
| [Content moderation](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-content-moderation-dashboard/README.md) | ReviewBay | Queue, policies, appeals, and automation | `#7C3AED` | [localhost:5173/content-moderation/overview](http://localhost:5173/content-moderation/overview) |
| [Data pipeline](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-data-pipeline-dashboard/README.md) | Conduit | Ingestion, transformations, quality, and lineage | `#D45060` | [localhost:5192/data-pipeline/overview](http://localhost:5192/data-pipeline/overview) |
| [Marketing command](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-marketing-command-center/README.md) | Marquee | Campaigns, audiences, content, and automation | `#3E0F8D` | [localhost:5193/marketing/overview](http://localhost:5193/marketing/overview) |
| [Document RAG](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-document-rag-dashboard/README.md) | Contextly | Ingestion, retrieval, citations, and evals | `#0F766E` | [localhost:5173/document-rag/overview](http://localhost:5173/document-rag/overview) |
| [Governance](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-governance-compliance-dashboard/README.md) | Charter | Inventories, risk, policies, and approvals | `#B0CDE6` | [localhost:5191/governance/overview](http://localhost:5191/governance/overview) |
| [LLM ops](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-llm-ops-dashboard/README.md) | Poluru LLM Ops | Traces, playground, evals, and cost | `#4338CA` | [localhost:5185/llm-ops/overview](http://localhost:5185/llm-ops/overview) |
| [ML training](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-ml-training-dashboard/README.md) | Kiln | Training runs, datasets, and GPU clusters | `#DE3E3E` | [localhost:5184/ml-training/overview](http://localhost:5184/ml-training/overview) |
| [Model evaluation](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-model-evaluation-dashboard/README.md) | Prism | Eval suites, leaderboards, and human review | `#FF8383` | [localhost:5186](http://localhost:5186) |
| [Prompt management](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-prompt-management-dashboard/README.md) | Prompt Bureau | Library, versions, evals, and releases | `#162E93` | [localhost:5187/prompt-management/overview](http://localhost:5187/prompt-management/overview) |
| [SaaS admin](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-saas-admin-dashboard/README.md) | Nexus | Tenants, billing, flags, and audit | `#059669` | [localhost:5188/saas-admin/overview](http://localhost:5188/saas-admin/overview) |
| [Support helpdesk](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-support-helpdesk-dashboard/README.md) | Relay | Inbox, SLA, macros, and copilot drafts | `#EA580C` | [localhost:5189](http://localhost:5189) |
| [Synthetic data studio](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/ai-synthetic-data-studio/README.md) | Poluru Synth Studio | Synthetic datasets, differential privacy, quality and TSTR evals | `#05339C` | [localhost:5194/synthetic-data/overview](http://localhost:5194/synthetic-data/overview) |
| [Enterprise dashboard](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/blob/main/enterprise-dashboard/README.md) | Poluru DC | Facilities, power, capacity, and tickets | `#30AFFF` | [localhost:5173](http://localhost:5173) |

**Port notes:** AgentPulse, Sightline, ReviewBay, Contextly, and Poluru DC use Vite’s default **5173** — run one at a time or pass `--port` to `npm run dev`. Marquee uses **5193**. Prism uses hash routes (`#/overview`). Several other apps also default to **5189** in `vite.config.js`; check the [full catalog](#all-template-folders) before running multiple demos.

Browse source for any template:

`https://github.com/poluru-labs/enterprise-react-free-ai-web-templates/tree/main/<folder-name>`

## Desk demos (dedicated dev ports)

Light Bootstrap desk UIs (Roboto + Lato, branded headers). Each folder sets an explicit dev port in `vite.config.js`:

| Folder | Product | Dev port |
| --- | --- | ---: |
| `ai-accessibility-auditor` | AuditDesk | 5207 |
| `ai-algorithmic-fairness-auditor` | ParityDesk | 5208 |
| `ai-assistive-learning-platform` | LearnDesk | 5209 |
| `ai-citation-verification-console` | CiteDesk | 5210 |
| `ai-data-provenance-explorer` | ProvDesk | 5211 |
| `ai-dataset-quality-inspector` | QualDesk | 5212 |
| `ai-disaster-resource-coordinator` | ReliefDesk | 5213 |
| `ai-inference-benchmarking-lab` | BenchDesk | 5214 |
| `ai-open-source-maintainer-workspace` | MaintDesk | 5215 |
| `ai-privacy-preserving-analytics` | PrivDesk | 5216 |
| `ai-rag-retrieval-quality-analyzer` | RqDesk | 5217 |
| `ai-research-reproducibility-workbench` | ReproDesk | 5218 |
| `ai-scientific-literature-mapper` | LitDesk | 5219 |

## All template folders

| Folder | Product / title | Dev port | Status |
| --- | --- | ---: | --- |
| `ai-accessibility-auditor` | AuditDesk | 5207 | App |
| `ai-agent-builder-studio` | Agent Builder Studio | 5189 | App |
| `ai-agent-monitoring-dashboard` | AgentPulse | 5173 | App |
| `ai-algorithmic-fairness-auditor` | ParityDesk | 5208 | App |
| `ai-api-gateway-dashboard` | API Gateway (starter shell) | 5189 | App |
| `ai-assistive-learning-platform` | LearnDesk | 5209 | App |
| `ai-citation-verification-console` | CiteDesk | 5210 | App |
| `ai-computer-vision-dashboard` | Sightline | 5173 | App |
| `ai-content-moderation-dashboard` | ReviewBay | 5173 | App |
| `ai-data-pipeline-dashboard` | Conduit | 5192 | App |
| `ai-data-provenance-explorer` | ProvDesk | 5211 | App |
| `ai-dataset-quality-inspector` | QualDesk | 5212 | App |
| `ai-disaster-resource-coordinator` | ReliefDesk | 5213 | App |
| `ai-document-processing-dashboard` | Pagewise | 5194 | App |
| `ai-document-rag-dashboard` | Contextly | 5173 | App |
| `ai-edge-inference-dashboard` | CareLine | 5195 | App |
| `ai-energy-optimization-dashboard` | GridPulse | 5196 | App |
| `ai-experimentation-platform` | VariantLab | 5197 | App |
| `ai-financial-risk-dashboard` | RiskPulse | 5198 | App |
| `ai-forecasting-planning-dashboard` | PlanPulse | 5199 | App |
| `ai-governance-compliance-dashboard` | Charter | 5191 | App |
| `ai-healthcare-operations-dashboard` | ClinicPulse | 5200 | App |
| `ai-human-in-the-loop-workspace` | ReviewLoop | 5201 | App |
| `ai-inference-benchmarking-lab` | BenchDesk | 5214 | App |
| `ai-knowledge-base-dashboard` | KnowPulse | 5202 | App |
| `ai-legal-contract-intelligence-dashboard` | ContractPulse | 5203 | App |
| `ai-llm-ops-dashboard` | Poluru LLM Ops | 5185 | App |
| `ai-marketing-command-center` | Marquee | 5193 | App |
| `ai-marketing-intelligence-dashboard` | Marketing Intelligence | 5189 | App |
| `ai-ml-training-dashboard` | Kiln | 5184 | App |
| `ai-model-evaluation-dashboard` | Prism | 5186 | App |
| `ai-open-source-maintainer-workspace` | MaintDesk | 5215 | App |
| `ai-personalization-dashboard` | Personalization | 5200 | App |
| `ai-privacy-preserving-analytics` | PrivDesk | 5216 | App |
| `ai-prompt-management-dashboard` | Prompt Bureau | 5187 | App |
| `ai-rag-retrieval-quality-analyzer` | RqDesk | 5217 | App |
| `ai-recommendation-engine-dashboard` | Recommendation Engine | 5189 | App |
| `ai-research-reproducibility-workbench` | ReproDesk | 5218 | App |
| `ai-robotics-fleet-dashboard` | Robotics Fleet | 5204 | App |
| `ai-saas-admin-dashboard` | Nexus | 5188 | App |
| `ai-scientific-literature-mapper` | LitDesk | 5219 | App |
| `ai-search-analytics-dashboard` | Search Analytics (starter shell) | 5189 | App |
| `ai-security-operations-center` | Security Operations | — | README stub only |
| `ai-supply-chain-control-tower` | Supply Chain Control Tower | 5205 | App |
| `ai-support-helpdesk-dashboard` | Relay | 5189 | App |
| `ai-synthetic-data-studio` | Poluru Synth Studio | 5194 | App |
| `ai-translation-operations-dashboard` | Translation Operations | 5206 | App |
| `ai-voice-operations-dashboard` | Voice Operations | 5189 | App (minimal shell) |
| `enterprise-dashboard` | Poluru DC | 5173 | App |

Ports come from each template’s `vite.config.js` where set; otherwise Vite defaults to **5173**. `ai-document-processing-dashboard` and `ai-synthetic-data-studio` both use **5194** — run one at a time.

## Getting started

Requires **Node.js 20+** (Node 18 works on several older templates).

```bash
git clone https://github.com/poluru-labs/enterprise-react-free-ai-web-templates.git
cd enterprise-react-free-ai-web-templates/ai-agent-monitoring-dashboard
npm install
npm run dev
```

Replace the folder name with any template from the tables above. Open that app’s local demo URL (see [Showcase templates](#showcase-templates) or the folder README). Production build:

```bash
npm run build
```

Each template has its own `package.json` — install and run inside that folder only.

| Script | Description |
| --- | --- |
| `npm run dev` | Vite development server |
| `npm test` | Vitest unit tests (where the template includes them) |
| `npm run build` | Production build |
| `npm run preview` | Preview the production build |

## Stack

Most templates share:

- React 18 + React Router 6 (**Poluru DC** uses React 19, Router 7, and TypeScript)
- Vite
- Bootstrap 5 + Bootstrap Icons (**Poluru DC** uses SCSS instead of Bootstrap; Desk demos use Roboto + Lato with light branded themes)
- [`@poluru-labs/enterprise-design-system-react`](https://www.npmjs.com/package/@poluru-labs/enterprise-design-system-react)
- Vitest + Testing Library + jsdom

Copy and mock data live in each app’s `src/data/`. Layout and brand color live in `src` CSS/SCSS and the header/shell components.

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

## Design system

Install dependencies inside each template folder. The React package is **`@poluru-labs/enterprise-design-system-react`**, pinned in that app’s `package.json`.

Source: [enterprise-design-system-react](https://github.com/poluru-labs/enterprise-design-system-react) · npm: [@poluru-labs/enterprise-design-system-react](https://www.npmjs.com/package/@poluru-labs/enterprise-design-system-react)

## License

MIT © 2026 [Subrahmanyam Poluru](https://polurus.com) / Poluru Labs. Check the upstream `LICENSE` before redistribution.
