# Webflyx (HyperNetwork – Docker Networking Project)

## Overview
Practice repo for **Docker networks and volumes**. Spins up **Postgres** and **Adminer** on a bridged network for local exploration. Hyperskill project.

## Features
- Counts words/characters
- Top-N words
- Report to stdout (optionally to file)

## Tech
- Docker
- Docker Compose
- Postgres
- Adminer

## How to run

```bash
docker compose up -d
docker ps
```
Adminer: http://localhost:8080
Use the credentials from your docker-compose.yml, e.g.:
- System: PostgreSQL
- Server: postgres
- User: postgres (or $POSTGRES_USER)
- Password: ******** ( $POSTGRES_PASSWORD)
- Database: webflyx (if set)

### Common commands
```bash
docker compose logs -f
docker exec -it <postgres_container> psql -U $POSTGRES_USER -d $POSTGRES_DB
docker compose down -v  # remove volumes
```
