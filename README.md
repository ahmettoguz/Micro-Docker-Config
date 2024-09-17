## 🚀🚀🚀 Dev Commands 🚀🚀🚀

```
docker-compose -p micro down
docker-compose -p micro up -d --build

docker-compose -p micro down reverse-proxy
docker-compose -p micro up -d reverse-proxy --build

docker-compose -p micro down frontend
docker-compose -p micro up -d frontend --build

docker-compose -p micro down backend
docker-compose -p micro up -d backend --build

docker-compose -p micro down email-service
docker-compose -p micro up -d email-service --build

docker-compose ls
```