docker-compose -p micro up -d --build
docker-compose -p micro down

docker-compose -p micro up -d frontend

docker-compose ls

depends on means run dependent module also even its not started by implicitly


-------------------------------------------- Release 1.1.0 --------------------------------------------
+ frontend react app is dockerized
+ backend spring boot app is dockerized
+ spring boot env variables adjusted
+ frontend can send request to backend
+ email service is available
+ email service has swagger documentation

- frontend and backend communication is established over url not docker
- backend do not have swagger documentation
- frontend cannot send email
- frontend do not have env variables
- ssl is not set up for backend and frontend
- backend service is available to public

- no database
- no database ui
- no database initializer

-------------------------------------------- Release 1.0.0 --------------------------------------------
+ frontend react app is dockerized
+ backend spring boot app is dockerized
+ spring boot env variables adjusted
+ frontend can send request to backend

- frontend do not have env variables
- frontend and backend communication is established over url not docker
- ssl is not set up for backend and frontend
- backend service is available to public
- email service is not available
- frontend cannot send email
