# FastAPI Real-World Projects

**Repository:** [github.com/poluru-labs/fastapi-realworld-projects](https://github.com/poluru-labs/fastapi-realworld-projects)

Hands-on **FastAPI** backends across three difficulty tracks (**58** project folders). Each app is self-contained with `app/`, `tests/`, `requirements.txt` / `pyproject.toml`, a `Dockerfile`, and a walkthrough README covering routes, validation, and common status codes. Many projects include **Pytest**, **Swagger** / **ReDoc**, and (on advanced apps) **Docker Compose**, **Postgres**, and **Alembic**. **MIT** license.

Part of the [Free UI Templates](../README.md) catalog.

## Structure

| Track | Folder | Count | Focus |
| --- | --- | ---: | --- |
| Beginner | `beginner/` | 22 | Versioned `/api/v1` CRUD, Pydantic validation, in-memory repos, Pytest |
| Intermediate | `intermediate/` | 20 | JWT auth, publishing workflows, chat, jobs, imports, richer domain rules |
| Advanced | `advanced/` | 16 (+ `starter`) | Multitenancy, WebSockets, billing, schedulers, event sourcing, IoT |

Work inside one project folder — there is no root monorepo `package.json` / shared install.

## Beginner projects

| Folder | Theme |
| --- | --- |
| `fastapi-hello-api` | Minimal API starter |
| `fastapi-todo` | Todos with filters and complete/reopen |
| `fastapi-notes` | Notes CRUD |
| `fastapi-bookmarks` | Bookmarks |
| `fastapi-recipes` | Recipe Box — filters, cuisines, featured flag |
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

Typical beginner layout: `app/main.py`, `core/`, `api/v1/endpoints/`, `schemas/`, `repositories/`, `services/`, plus `tests/api/v1/`.

## Intermediate projects

| Folder | Theme |
| --- | --- |
| `authentication-services` | Auth-focused service patterns |
| `fastapi-blog` | JWT login, drafts vs published (404 hiding), comments |
| `fastapi-ecommerce` | Commerce flows |
| `fastapi-inventory` | Inventory |
| `fastapi-job-board` | Job board |
| `fastapi-helpdesk` | Helpdesk / tickets |
| `fastapi-team-tasks` | Team tasks |
| `fastapi-subscriptions` | Subscriptions |
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

## Advanced projects

| Folder | Theme |
| --- | --- |
| `fastapi-multitenant-saas` | Tenants via `X-Tenant-Slug`, roles, plan limits, Postgres/Alembic |
| `fastapi-distributed-chat` | Distributed chat |
| `fastapi-distributed-orders` | Distributed orders |
| `fastapi-distributed-scheduler` | Distributed scheduler |
| `fastapi-collaborative-editor` | Collaborative editing |
| `fastapi-realtime-analytics` | Realtime analytics |
| `fastapi-event-sourced-wallet` | Event-sourced wallet |
| `fastapi-workflow-engine` | Workflow engine |
| `fastapi-webhook-delivery` | Webhook delivery |
| `fastapi-usage-billing` | Usage billing |
| `fastapi-ticket-booking` | Ticket booking |
| `fastapi-rate-limiter` | Rate limiting |
| `fastapi-resumable-files` | Resumable uploads |
| `fastapi-location-tracking` | Location tracking |
| `fastapi-iot-telemetry` | IoT telemetry |
| `fastapi-experimentation` | Experimentation / feature flags |
| `starter` | Advanced starter scaffold |

## Getting started

Python 3.11+ recommended (check each project’s `pyproject.toml`).

```bash
git clone https://github.com/poluru-labs/fastapi-realworld-projects.git
cd fastapi-realworld-projects/beginner/fastapi-recipes
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -e ".[dev]"
cp .env.example .env        # when the file exists
uvicorn app.main:app --reload
```

| URL / command | Purpose |
| --- | --- |
| http://127.0.0.1:8000/docs | Swagger UI |
| http://127.0.0.1:8000/redoc | ReDoc |
| `pytest -v` | Run the project’s tests |
| `docker build -t fastapi-recipes .` then `docker run --rm -p 8000:8000 fastapi-recipes` | Containerized run |

Advanced apps with databases often use `docker-compose.yml` (Postgres) and Alembic migrations — follow that folder’s README.

## What you practice

- FastAPI routers under `/api/v1`, Pydantic models, and OpenAPI examples
- Layered design: endpoints → services → repositories
- Clear HTTP semantics (`401` / `403` / `404` / `409` / `422`)
- Auth (JWT + refresh), tenancy headers, background work, and realtime patterns as you move up tracks

## License

**MIT** on this collection. Check the upstream `LICENSE` before redistribution.
