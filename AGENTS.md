# Base44 Dev Environment

## Project Overview
This is a **static single-page website** (`index.html`) for "مزون دلاویز" (Delaviz Mezon), a Persian/Farsi landing page for a children's and mother's clothing tailoring business. It was originally a GitHub Pages site (see `CNAME` → `delavizmezon.ir`).

## Tech Stack
- Plain HTML + CSS (inline in `index.html`), no JavaScript framework, no build step, no dependencies.

## Running
```
docker compose -f docker-compose.base44.yml up -d
```
Serves `index.html` via nginx on host port 3000. No backend, no database, no secrets required.

## Verification
- `curl http://localhost:3000/` returns the HTML page.
- The page renders RTL Persian content with sections: hero, services, portfolio, process, contact.
