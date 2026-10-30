# Enterprise Angular Free AI Web Templates

**Repository:** [github.com/poluru-labs/enterprise-angular-free-ai-web-templates](https://github.com/poluru-labs/enterprise-angular-free-ai-web-templates)

**35** standalone **Angular 21** demos for AI dashboards, ops consoles, and admin workspaces. Each `ai-*` folder is its own app with **`@poluru-labs/enterprise-design-system-angular`**, light UI with per-template brand colors, **Roboto + Lato** on EDS dashboards, demo data, **signals + `OnPush`** on showcase apps, and **`ng build`** / **`ng test --watch=false`**. **MIT** license.

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

| Script | Description |
| --- | --- |
| `npm start` | Angular dev server |
| `npm run build` | Production build |
| `npm test -- --watch=false` | Unit tests |

Customize brand tokens in `src/styles.scss`, shell and demo data in `src/app/app.ts` / `app.html`, and router apps under `src/app/features/…`.

## Design system

Templates use **[`@poluru-labs/enterprise-design-system-angular`](https://www.npmjs.com/package/@poluru-labs/enterprise-design-system-angular)** — a token-driven Angular component library (standalone `eds-*` components, design tokens, light/dark theming via `EdsThemeService`, Storybook docs).

Source: [enterprise-design-system-angular](https://github.com/poluru-labs/enterprise-design-system-angular)

### Install (in a new Angular app)

```bash
npm install @poluru-labs/enterprise-design-system-angular
```

**Peer dependencies:** `@angular/common`, `@angular/core`, and `@angular/platform-browser` (`^19 || ^20 || ^21`), plus `rxjs` (`^7.8`).

### Styles

Include the package styles in `angular.json` (or your global stylesheet entry):

```json
"styles": [
  "@poluru-labs/enterprise-design-system-angular/tokens.css",
  "@poluru-labs/enterprise-design-system-angular/styles.css",
  "src/styles.scss"
]
```

Templates typically override brand tokens in `src/styles.scss` under `:root` (for example `--eds-color-brand`).

### Usage

```ts
import { Component } from '@angular/core';
import {
  EdsButtonComponent,
  EdsThemeService,
  ToastService,
} from '@poluru-labs/enterprise-design-system-angular';

@Component({
  selector: 'app-root',
  standalone: true,
  imports: [EdsButtonComponent],
  template: `
    <eds-button (click)="notify()">Save</eds-button>
  `,
})
export class AppComponent {
  constructor(
    private theme: EdsThemeService,
    private toast: ToastService,
  ) {}

  toggleTheme() {
    this.theme.toggleTheme();
  }

  notify() {
    this.toast.show({ title: 'Saved', variant: 'success' });
  }
}
```

Optional dark theme:

```html
<html class="eds-theme-dark">
  <!-- or EdsThemeService.setTheme('dark') -->
</html>
```

### What the library provides

- Angular 19+ standalone components with `eds-*` selectors
- Shared tokens for color, typography, spacing, radius, elevation, and motion
- Theme support (light/dark) via `EdsThemeService`
- Built-in icons, overlays (modal, drawer, toast), forms, data display, and navigation primitives

Explore components in the design-system repo with `npm run storybook` (port **6008**).

## License

**MIT** on this collection. Check the upstream `LICENSE` before redistribution.
