# Enterprise React Free AI Web Templates

**Repository:** [github.com/poluru-labs/enterprise-react-free-ai-web-templates](https://github.com/poluru-labs/enterprise-react-free-ai-web-templates)

Production-shaped **React** templates for AI dashboards, ops consoles, and admin workspaces. Each folder is an independent **Vite** app with **`@poluru-labs/enterprise-design-system-react`**, **Bootstrap 5**, mock data under `src/data/`, and **Vitest** where included. **MIT** license.

Part of the [Free UI Templates](../README.md) catalog.

## Templates

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

## Design system

Install dependencies inside each template folder. The React package is **`@poluru-labs/enterprise-design-system-react`**, pinned in that app’s `package.json`.

## License

**MIT** on this collection. Check the upstream `LICENSE` before redistribution.
