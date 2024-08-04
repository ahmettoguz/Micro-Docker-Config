docker-compose -p micro up -d --build
docker-compose -p micro down

docker-compose -p micro up -d frontend

docker-compose ls

depends on means run dependent module also even its not started by implicitly