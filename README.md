# Automated Code Assessment (Prototype)

## Quick start

Requirements: Docker & Docker Compose.

```
docker compose up --build
```

Backend: http://localhost:3000
Runner: http://localhost:5001
Frontend (static placeholder): http://localhost:5173

## Flow
- Register and login to obtain a JWT.
- List assignments: GET /assignments
- Submit a ZIP with `solution.py` via POST /submissions (multipart, fields: assignmentId, file)
- Poll GET /submissions/:id for status and results.

## Notes
- Prototype supports Python via pytest. Architecture allows more languages via adapters.
- Data stored in `./data` directory. Sample tests in `./tasks`.








