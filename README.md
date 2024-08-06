<h1 id="top" align="center">🚢 Release Version 1.1.0 </h1> 

<br/>

## 🔍 Table of Contents

- [Service Versions](#service-versions)
- [Features](#features)
- [Limitations](#limitations)
- [System Startup](#system-startup)
 
<br/>

<h2 id="service-versions">🧩 Service Versions</h2> 

| Service               | Version                                                                                                                                                                           |
|-----------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Micro-Docker-Config   | [![.](https://img.shields.io/badge/1.1.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/1.1.0)   |
| Micro-Backend         | [![.](https://img.shields.io/badge/1.0.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Backend/tree/release/1.0.0)         |
| Micro-Email-Service   | [![.](https://img.shields.io/badge/1.0.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Email-Service/tree/release/1.0.0)   |
| Micro-Frontend        | [![.](https://img.shields.io/badge/1.0.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Frontend/tree/release/1.0.0)        |

<br/>

<h2 id="features">🔥 Features</h2>

+ frontend react app is dockerized
+ backend spring boot app is dockerized
+ spring boot env variables adjusted
+ frontend can send request to backend
+ email service is available
+ email service has swagger documentation

<br/>

<h2 id="limitations">🚧 Limitations</h2>

- frontend and backend communication is established over url not docker
- backend do not have swagger documentation
- frontend cannot send email
- frontend do not have env variables
- ssl is not set up for backend and frontend
- backend service is available to public
- no database
- no database ui
- no database initializer

<br/>
  
<h2 id="system-startup">🚀 System Startup</h2> 

```
docker-compose -p micro up -d --build

docker-compose -p micro down

docker-compose ls
```

[🔝](#top)
