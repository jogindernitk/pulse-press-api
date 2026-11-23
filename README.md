# PulsePress API

Backend REST API for **PulsePress**, built with FastAPI, PostgreSQL, and `uv`.

## Quickstart

1. **Start PostgreSQL via Docker:**
   ```bash
   docker run --name pgdb --rm -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=postgres -e POSTGRES_DB=pulsepress -p 5432:5432 -d postgres
   ```
2. **Install Dependencies & Run:**
   ```bash
   uv sync
   uv run alembic upgrade head
   uv run uvicorn app.main:app --reload
   ```
   *Access API docs at `http://localhost:8000/docs`.*
