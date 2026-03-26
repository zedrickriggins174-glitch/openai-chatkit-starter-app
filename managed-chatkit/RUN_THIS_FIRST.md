# Managed ChatKit quick run

## 1) Create env file
In `managed-chatkit/`, copy `.env.local.example` to `.env.local` and set:

- `OPENAI_API_KEY`
- `VITE_CHATKIT_WORKFLOW_ID`

## 2) Start the app
```bash
cd managed-chatkit
npm install
npm run dev
```

## 3) Expected ports
- Frontend: `http://127.0.0.1:3000` (or the Codespaces forwarded port)
- Backend: `http://127.0.0.1:8000`

## 4) Session flow
The frontend posts to `/api/create-session`, and Vite proxies `/api/*` to the FastAPI backend.

## 5) Important
Do **not** put the real OpenAI secret in any `VITE_` variable.
