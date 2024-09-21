## 🚀🚀🚀 Deploy Commands 🚀🚀🚀

```
sudo docker compose -p micro down
sudo docker compose -p micro up -d --build

sudo docker compose -p micro down reverse-proxy
sudo docker compose -p micro up -d reverse-proxy --build

sudo docker compose -p micro down frontend
sudo docker compose -p micro up -d frontend --build

sudo docker compose -p micro down backend
sudo docker compose -p micro up -d backend --build

sudo docker compose -p micro down email-service
sudo docker compose -p micro up -d email-service --build

sudo docker compose ls
sudo docker ps -a
sudo docker logs reverse-proxy
```