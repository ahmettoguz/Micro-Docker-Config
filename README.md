<h1 id="top" align="center">🚢 Release Version 1.1.0 </h1> 

<br/>

## 🔍 Table of Contents

- [Service Versions](#service-versions)
- [Features](#features)
- [Next Release Features](#next-release-features)
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

### Frontend
+ The application has been Dockerized.
+ frontend can send request to backend

### Backend
+ The application has been Dockerized.
+ Environment variables have been adjusted.

### Email Service
+ Service is available.
+ Swagger documentation has been integrated.


<br/>

<h2 id="next-release-features">🚧 Next Release Features</h2>

### Frontend

- Env variable support.
- Internal communication between backend service.
- TLS/HTTPS support.
- Email service integration.


### Backend

- Internal communication with frontend.
- TLS/HTTPS support.
- Swagger api documentation.

### Email Service

- Communication with frontend.
- Internal communication with frontend.

<br/>
  
<h2 id="system-startup">🚀 System Startup</h2> 

```
docker-compose -p micro up -d --build

docker-compose -p micro down

docker-compose ls
```

[🔝](#top)
