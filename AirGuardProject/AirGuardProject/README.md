# AirGuard — Air Quality Index Prediction System

A full-stack recreation of the AirGuard interface shown in the supplied reference video. The project keeps the visible navigation, dashboard cards, AQI prediction workflow, analytics charts, model comparison, prediction history and project information pages.

## Project structure

- `frontend/` — React + Vite application
- `backend/` — FastAPI machine-learning API
- `data/` — reserved for your real air-quality CSV/dataset

## Run frontend

```bash
cd frontend
npm install
npm run dev
```

Open the Vite URL shown in the terminal.

## Run backend

Create a Python virtual environment if desired, then:

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```

The API runs at `http://127.0.0.1:8000`.

## Important

The reference video only exposes the frontend/demo behavior. Therefore this version uses a reproducible demo regression model in the backend rather than claiming to reproduce an unseen original Lovable model or dataset. When the original dataset/model becomes available, replace the demo training section in `backend/main.py` with the actual trained pipeline and keep the UI unchanged.
