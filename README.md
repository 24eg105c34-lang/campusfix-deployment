# CampusFix Deployment
This repository contains the Docker Compose deployment configuration for CampusFix. It builds the frontend and backend directly from their folders in the [`campusfix-fullstack`](https://github.com/24eg105c34-lang/campusfix-fullstack) repository.

## Run the full project
From this repository's root:
```bash
docker compose up --build
```
Frontend: http://localhost:8081  
Backend API: http://localhost:8080/api/complaints

For a real public deployment, use a platform supporting static hosting and Java containers (for example, Render, Railway, or a VPS). Configure `API_BASE` in `campusfix-frontend/app.js` to the public backend URL. Set up a managed PostgreSQL database, HTTPS, environment secrets, restricted CORS, and admin authentication before production use.