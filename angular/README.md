# Enterprise Angular Free AI Web Templates

**Repository:** [github.com/poluru-labs/enterprise-angular-free-ai-web-templates](https://github.com/poluru-labs/enterprise-angular-free-ai-web-templates)

**35** standalone **Angular 21** demos for AI dashboards, ops consoles, and admin workspaces. Uses **`@poluru-labs/enterprise-design-system-angular`**, light UI with per-template brand colors, **Roboto + Lato** on EDS dashboards, demo data, **signals + `OnPush`** on showcase apps, and **`ng build`** / **`ng test --watch=false`** in each project. **MIT** license.

Part of the [Free UI Templates](../README.md) catalog.

## Sample of templates

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

## Getting started

Node.js 20+ LTS.

```bash
git clone https://github.com/poluru-labs/enterprise-angular-free-ai-web-templates.git
cd enterprise-angular-free-ai-web-templates/ai-prompt-playground
npm install
npm start
```

Default URL: `http://localhost:4200/`. Run multiple demos with `ng serve --port 4215` (or another free port).

Customize brand tokens in `src/styles.scss`, shell and demo data in `src/app/app.ts` / `app.html`, and router apps under `src/app/features/…`.

## Design system

Install dependencies inside each template folder. The Angular package is **`@poluru-labs/enterprise-design-system-angular`**, pinned in that app’s `package.json`.

## License

**MIT** on this collection. Check the upstream `LICENSE` before redistribution.
