# FastAPI Real-World Projects

**Repository:** [github.com/poluru-labs/fastapi-realworld-projects](https://github.com/poluru-labs/fastapi-realworld-projects)

Hands-on **FastAPI** backends across three difficulty tracks (**72** project folders: **25** beginner, **25** intermediate, **22** advanced including `starter`). Each app is self-contained with `app/`, `tests/`, `pyproject.toml` (and often `requirements.txt`), a `Dockerfile`, and a project README with routes, auth headers, and walkthroughs. Most samples expose long-form **OpenAPI** narratives in `app/main.py`, plus **Swagger** / **ReDoc**, **Pytest**, and **Ruff**. Advanced apps add async SQLAlchemy, **Alembic**, optional **Docker Compose** (Postgres), and domain-specific patterns (tenancy, WebSockets, billing, policy engines, and more). **MIT** license.

Part of the [Free UI Templates](../README.md) catalog.

## Structure

| Track | Folder | Count | Focus |
| --- | --- | ---: | --- |
| Beginner | `beginner/` | 25 | Versioned `/api/v1`, Pydantic validation, in-memory or SQLite repos, Pytest |
| Intermediate | `intermediate/` | 25 | JWT (and API keys where noted), publishing workflows, integrations, richer domain rules |
| Advanced | `advanced/` | 22 | Multitenancy, realtime, schedulers, event sourcing, identity/RAG/agent orchestration, `starter` scaffold |

Work inside one project folder — there is no root monorepo install; copy `advanced/starter` when bootstrapping a new advanced service.

## Beginner projects

| Folder | Theme |
| --- | --- |
| `fastapi-hello-api` | Minimal API starter |
| `fastapi-todo` | Todos with filters and complete/reopen |
| `fastapi-notes` | Notes CRUD |
| `fastapi-bookmarks` | Bookmarks |
| `fastapi-recipes` | Recipe box — filters, cuisines, featured flag |
| `fastapi-book-catalog` | Book catalog |
| `fastapi-product-catalog` | Product catalog |
| `fastapi-contact-book` | Contacts |
| `fastapi-expense-tracker` | Expenses |
| `fastapi-habit-tracker` | Habits |
| `fastapi-journal` | Journal entries |
| `fastapi-flashcards` | Flashcards |
| `fastapi-quiz` | Quizzes |
| `fastapi-polls` | Polls |
| `fastapi-events` | Events |
| `fastapi-gradebook` | Gradebook |
| `fastapi-movie-watchlist` | Movie watchlist |
| `fastapi-support-tickets` | Support tickets |
| `fastapi-url-shortener` | URL shortener |
| `fastapi-unit-converter` | Unit converter |
| `fastapi-text-analyzer` | Text analysis |
| `fastapi-calculator-mock` | Calculator mock |
| `fastapi-file-upload` | Multipart uploads, size limits |
| `fastapi-image-metadata` | Image metadata (Pillow) |
| `fastapi-weather` | Locations, current/forecast weather |

Typical layout: `app/main.py`, `core/`, `api/v1/endpoints/`, `schemas/`, `repositories/`, `services/`, `tests/api/v1/`.

## Intermediate projects

| Folder | Theme |
| --- | --- |
| `authentication-services` | Auth-focused service patterns |
| `fastapi-blog` | JWT, drafts vs published (404 hiding), comments |
| `fastapi-ecommerce` | Commerce flows |
| `fastapi-inventory` | Inventory |
| `fastapi-job-board` | Job board |
| `fastapi-helpdesk` | Helpdesk / tickets |
| `fastapi-team-tasks` | Team tasks, platform vs team roles |
| `fastapi-subscriptions` | Subscriptions and plans |
| `fastapi-appointments` | Appointments |
| `fastapi-event-registration` | Event registration |
| `fastapi-restaurant-orders` | Restaurant orders |
| `fastapi-personal-finance` | Personal finance |
| `fastapi-learning` | Learning / courses |
| `fastapi-social-feed` | Social feed |
| `fastapi-realtime-chat` | Realtime chat |
| `fastapi-notifications` | Notifications |
| `fastapi-webhook-inbox` | Webhook inbox |
| `fastapi-csv-import` | CSV import |
| `fastapi-media-processing` | Media processing |
| `fastapi-report-generator` | Report generation |
| `fastapi-api-aggregator` | JWT, sources, parallel mock aggregates, idempotency |
| `fastapi-api-keys` | Hashed API keys, scopes, JWT or `X-Api-Key` |
| `fastapi-document-library` | Folders, documents, publish/revisions, search |
| `fastapi-feature-flags` | Rollouts, allowlists, runtime evaluate token |
| `fastapi-uptime-monitor` | Mock probes, pause, public status pages |

## Advanced projects

| Folder | Theme |
| --- | --- |
| `starter` | Lean advanced scaffold (health, Alembic, async SQLAlchemy) |
| `fastapi-multitenant-saas` | JWT + `X-Tenant-Slug`, roles, plan limits |
| `fastapi-multitenant-rag` | Tenant-scoped RAG ingest, chunking, query |
| `fastapi-policy-authorization` | RBAC/ABAC rules, `/policy/evaluate`, protected documents |
| `fastapi-identity-gateway` | OAuth-style clients, token, userinfo, introspection |
| `fastapi-agent-workflows` | Agent/tool step workflows, idempotent runs |
| `fastapi-code-execution` | Sandbox policy, runner key, idempotent code runs |
| `fastapi-experimentation` | A/B experiments, assignments, idempotent events |
| `fastapi-workflow-engine` | Workflow definitions, instances, transitions |
| `fastapi-distributed-chat` | Distributed chat |
| `fastapi-distributed-orders` | Distributed orders |
| `fastapi-distributed-scheduler` | Distributed scheduler |
| `fastapi-collaborative-editor` | Collaborative editing |
| `fastapi-realtime-analytics` | Streams, metrics, alerts |
| `fastapi-event-sourced-wallet` | Event-sourced wallet |
| `fastapi-webhook-delivery` | Webhook delivery |
| `fastapi-usage-billing` | Usage meters, subscriptions, invoices |
| `fastapi-ticket-booking` | Ticket booking |
| `fastapi-rate-limiter` | Rate limits and client policies |
| `fastapi-resumable-files` | Resumable multipart uploads |
| `fastapi-location-tracking` | Trackers, geofences, trails |
| `fastapi-iot-telemetry` | Devices, telemetry, alerts |

## Getting started

Python **3.11+** (see each project’s `pyproject.toml`).

```bash
git clone https://github.com/poluru-labs/fastapi-realworld-projects.git
cd fastapi-realworld-projects/beginner/fastapi-recipes
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -e ".[dev]"
cp .env.example .env        # when present
uvicorn app.main:app --reload
```

| URL / command | Purpose |
| --- | --- |
| http://127.0.0.1:8000/docs | Swagger UI (read `app/main.py` description block too) |
| http://127.0.0.1:8000/redoc | ReDoc |
| `pytest -v` | Project tests (often in-memory SQLite in `tests/conftest.py`) |
| `ruff check app tests` | Lint (Alembic versions often excluded) |
| `alembic upgrade head` | Apply migrations (advanced / DB-backed apps) |
| `python -m scripts.seed_data` | Seed demo data when the project provides it |
| `docker compose up --build` | Postgres + API on many advanced samples |

## What you practice

- Routers under `/api/v1`, Pydantic models, and OpenAPI tags plus long API descriptions
- Layered design: endpoints → services → repositories; `AppError` → `{"detail": "..."}`
- HTTP semantics (`401` / `403` / `404` / `409` / `413` / `422`)
- Auth patterns: JWT, refresh rotation, API keys, admin/runner keys, tenant headers, OAuth-shaped tokens
- Data: async SQLAlchemy, Alembic, seeds, idempotency headers, background and realtime patterns on higher tracks

## License

**MIT** on this collection. Check the upstream `LICENSE` before redistribution.
