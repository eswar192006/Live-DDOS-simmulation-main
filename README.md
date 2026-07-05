# Live DDoS Simulation

Lightweight DDoS attack simulation project with a FastAPI backend and a small frontend.

## Repository structure

- `backend/` — FastAPI app and tests
- `frontend/` — static frontend using Vite
- `data/` — GeoIP database

## Quickstart

Prerequisites: Python 3.9+, Node.js (for frontend), `pip`.

Backend (API):

1. Create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

2. Install dependencies and run the server:

```bash
pip install -r backend/requirements.txt
uvicorn backend.app.main:app --reload --host 0.0.0.0 --port 8000
```

Frontend (dev):

```bash
cd frontend
npm install
npm run dev
```

Run tests (backend):

```bash
pip install -r backend/requirements.txt
pytest -q
```

## License
MIT
