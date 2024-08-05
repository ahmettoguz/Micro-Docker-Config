## Running services
```
docker-compose -p micro up -d --build

docker-compose -p micro down

docker-compose -p micro up -d frontend

docker-compose ls
```

<hr/> 
<br/>

<h2 id="release/1.1.0">Release 1.1.0</h2> 

| Service               | Version                                                                                                                                                                           |
|-----------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Micro-Docker-Config   | [![.](https://img.shields.io/badge/1.1.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/1.1.0)   |
| Micro-Backend         | [![.](https://img.shields.io/badge/1.1.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Backend/tree/release/1.0.0)         |
| Micro-Email-Service   | [![.](https://img.shields.io/badge/1.1.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Email-Service/tree/release/1.0.0)   |
| Micro-Frontend        | [![.](https://img.shields.io/badge/1.1.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Frontend/tree/release/1.0.0)        |

### Features

+ frontend react app is dockerized
+ backend spring boot app is dockerized
+ spring boot env variables adjusted
+ frontend can send request to backend
+ email service is available
+ email service has swagger documentation

### Limitations

- frontend and backend communication is established over url not docker
- backend do not have swagger documentation
- frontend cannot send email
- frontend do not have env variables
- ssl is not set up for backend and frontend
- backend service is available to public
- no database
- no database ui
- no database initializer

<hr/>