# AgriConnect MVP (Minimal Full-stack Scaffold)

This repo is a minimal, ready-to-run scaffold for the AgriConnect-inspired farmer platform MVP.
It includes:
- Backend: Node.js + Express + PostgreSQL (via Docker Compose).
- Frontend: React (Vite) + Material UI.
- Dockerfiles and docker-compose for local dev.
- Basic endpoints: auth (phone/email stub), farms CRUD, planting records, weather proxy (requires API key).
- CI: basic GitHub Actions workflow.

## Quickstart (Local with Docker Compose)

1. Copy `.env.example` to `.env` and set the values (especially WEATHER_API_KEY).
2. From repo root:
```bash
docker-compose up --build
```
3. Frontend should be available at http://localhost:3000
   Backend API at http://localhost:4000

## What I delivered
- A working minimal scaffold (not production hardened).
- All files are provided so you can push to a GitHub repo directly.
- To deploy: push to GitHub then connect to your host (Vercel/Netlify for frontend, Heroku/AWS/GCP/Render for backend), or use Docker images.

## Next steps (recommended)
- Add real authentication (password hashing, verification).
- Wire Postgres persistence and run migrations.
- Add real weather API key and extend routes.
- Add tests and improve CI/CD.

