<h1 id="top" align="center">🚢 Release Version 3.2.0 </h1> 

<br/>

## 🔍 Table of Contents

- [Service Versions](#service-versions)
- [Features](#features)
- [Next Release Features](#next-release-features)
- [System Links](#system-links)
- [System Preperation](#system-preperation)
- [System Startup](#system-startup)
 
<br/>

<h2 id="service-versions">🧩 Service Versions</h2> 

| Service               | Version                                                                                                                                                                           |
|-----------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Micro-Docker-Config   | [![.](https://img.shields.io/badge/3.2.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/3.2.0)   |
| Micro-Backend         | [![.](https://img.shields.io/badge/1.3.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Backend/tree/release/1.3.0)         |
| Micro-Email-Service   | [![.](https://img.shields.io/badge/1.2.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Email-Service/tree/release/1.2.0)   |
| Micro-Frontend        | [![.](https://img.shields.io/badge/2.3.1-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Frontend/tree/release/2.3.1)        |

<br/>

<h2 id="features">🔥 Features</h2>

### Micro Docker Config

+ **Centralized TLS Security:** Centralized TLS certificate configuration across all services.
+ **Auto-Renewal of Trusted TLS Certificates:** Automatic renewal of trusted TLS certificates to ensure uninterrupted security in production environments.
+ **Trusted TLS Certificates:** Secure communication between services using trusted SSL certificates managed by Traefik for production environment.
+ **Self-Signed TLS Certificates:** Secure communication between services using self-signed SSL certificates managed by Traefik for local development.
+ **Traefik Integration:** Traefik integrated for networking.
+ **Traefik Load Balancing:** Load balancing configured through Traefik for improved scalability and also local service development.
+ **Traefik Router:** Routing configured through Traefik for service communication without exposing port to public.
+ **Traefik Dashboard:** Dashboard integrated for monitoring and managing Traefik services, routers and prefixes.
+ **Docker-Compose Configuration:** Comprehensive Docker-Compose configuration for managing service orchestration.

### Micro Frontend

+ **Custom Modal:** Includes a custom modal component with configurable actions to enhance user interaction.
+ **Global State Management:** Redux implementation for consistent state handling across the application.
+ **Persistent Data:** Language, theme mode, and theme schema are stored in localStorage.
+ **Internationalization:** Language support with i18n for a multilingual user experience.
+ **Custom Scrollbar Design:** Custom scrollbar styling to match the application's aesthetic.
+ **Floating Action Button:** A "Go to Top" button for improved navigation.
+ **Multi-Message Snackbar:** Support for displaying multiple snackbars using notistack.
+ **Professional UI/UX:** Modern user interface and experience.
+ **Input Validation:** Enhanced validation support for user inputs.
+ **Dark/Light Theme Mode:** Toggle between dark and light modes.
+ **Theme Schema Customization:** Toggle between default and custom theme schema.
+ **Custom Theme:** Added support for custom themes.
+ **Responsive Design:** Optimized for different screen sizes and devices.
+ **Material-UI Integration:** Extensive use of Material-UI components.
+ **Environment Variables:** Support for environment variables to manage configurations.
+ **Dockerization:** The application is containerized for consistent deployment and scaling.

### Micro Backend

+ **Postman Endpoint Collection:** Postman collection added for ensure validation of all API endpoints.
+ **Swagger Documentation:** Comprehensive API documentation integrated for documentation and testing purposes.
+ **Environment Configuration:** Configurations have been adjusted for enhanced flexibility.
+ **Dockerization:** The application is containerized for consistent deployment and scaling.

### Micro Email Service

+ **Postman Endpoint Collection:** Postman collection added for ensure validation of all API endpoints.
+ **Swagger Documentation:** Comprehensive API documentation integrated for documentation and testing purposes.
+ **Environment Configuration:** Configurations have been adjusted for enhanced flexibility.
+ **Dockerization:** The application is containerized for consistent deployment and scaling.
  
<br/>

<h2 id="next-release-features">🚧 Next Release Features</h2>

### Frontend
- Animated counter
- Scroll reveal

<br/>

<h2 id="system-links">🔗 System Links</h2> 

| Service            | URL                                                        |
|--------------------|------------------------------------------------------------|
| Frontend           | https://sendsphere.com.tr/                                 |
| Traefik Dashboard  | https://sendsphere.com.tr/traefik/dashboard/#/             |
| Backend Swagger UI | https://sendsphere.com.tr/backend/sw/swagger-ui/index.html |
| Email Swagger UI   | https://sendsphere.com.tr/email/sw/swagger-ui/index.html   |

<br/>

<h2 id="system-preperation">🔧 System Preperation</h2>

<br/>

<h3 id="developer-mode">🧪 Developer Mode</h3>

#### Micro Docker Config

* Update the domain name in the `traefik-conf/traefik-dynamic.yml` file, replacing current domain name with your domain name such as localhost.
* Place email address to `traefik-conf/treafik.yml`.

<br/>

#### Micro Frontend

* To change system configs such as endpoint urls, modify `.env` file.
  
<br/>

#### Micro Email Service

* Place credentials in the `application-dev.properties` file.

<br/>

<h3 id="production-mode">⚡Production Mode</h3> 

#### Micro Docker Config

* Obtain a domain name.
* Update the domain name in the `traefik-conf/traefik-dynamic.yml` file, replacing current domain name with your domain.
* Place email address to `traefik-conf/treafik.yml`.
* Change permission of the `/crt/acme.json` file with `chmod 600`.

<br/>

#### Micro Frontend

* To change system configs such as endpoint urls, modify `.env` file.
  
<br/>

#### Micro Backend

* Copy `application-dev.properties` to create `application-prod.properties`.
* Change `app.var.appMode` to `prod`.
* Change `server.port` to `80`.

<br/>

#### Micro Email Service

* Go to your Google Account settings at [`myaccount.google.com`](https://myaccount.google.com/).
* In the navigation panel, select [`Security`](https://myaccount.google.com/security).
* Under `How you sign in to Google`, select `2-Step Verification`.
* Add your phone number as a verification method.
* Go to  [`myaccount.google.com/u/1/apppasswords`](https://myaccount.google.com/u/1/apppasswords) and generate a new app password.
* Copy `application-dev.properties` to create `application-prod.properties`.
* Change `app.var.appMode` to `prod`.
* Change `server.port` to `80`.
* Place credentials.

<br/>
  
<h2 id="system-startup">🚀 System Startup</h2>

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
```

### [🔝](#top)
