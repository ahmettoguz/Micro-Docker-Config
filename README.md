## Dev Commands

```
docker compose -p micro build
docker compose -p micro up -d
docker compose -p micro up -d --build
docker compose -p micro down

docker compose -p micro build reverse-proxy
docker compose -p micro up -d reverse-proxy
docker compose -p micro up --build -d reverse-proxy
docker compose -p micro down reverse-proxy

docker compose -p micro build frontend
docker compose -p micro up -d frontend
docker compose -p micro up --build -d frontend
docker compose -p micro down frontend

docker compose -p micro build backend
docker compose -p micro up -d backend
docker compose -p micro up --build -d backend
docker compose -p micro down backend

docker compose -p micro build email-service
docker compose -p micro up -d email-service
docker compose -p micro up --build -d email-service
docker compose -p micro down email-service

docker exec -it micro-backend-container /bin/sh
docker inspect micro-backend-container
docker logs micro-backend-container

cls
```