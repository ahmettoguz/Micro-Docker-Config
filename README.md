<h1 id="top" align="center">Micro <br/> Docker Config</h1> 

<br>

<div align="center">
    <img width=300 src="assets/banner/banner.png">
</div>

## 🔍 Table of Contents

- [About Project](#intro)
- [Technologies](#technologies)
- [Features](#features)
- [Releases](#releases)
- [Treafik Dashboard](#traefik-dashboard)
- [System Links](#system-links)
- [System Preperation](#system-preperation)
- [System Startup](#system-startup)
- [Contributors](#contributors)
 
<br/>

<h2 id="intro">📌 About Project</h2> 

This project seeks to architect a cohesive microarchitecture that integrates frontend and backend systems, incorporates email services, manages databases, implements automated testing, utilizes Docker for containerization, applies TLS security protocols, and configures reverse proxies. 

<br/>

<h2 id="technologies">☄️ Technologies</h2>

### DevOps

&nbsp; [![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)

&nbsp; [![Traefik](https://img.shields.io/badge/Traefik-24A1C1?style=for-the-badge&logo=traefikproxy&logoColor=black)](https://traefik.io/)

### Web Server

&nbsp; [![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)](https://www.nginx.com/)

&nbsp; [![Apache Tomcat](https://img.shields.io/badge/apache%20tomcat-%23F8DC75.svg?style=for-the-badge&logo=apache-tomcat&logoColor=black)](https://tomcat.apache.org/)

### Backend

&nbsp; [![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)](https://www.java.com/)

&nbsp; [![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)](https://spring.io/)

&nbsp; [![Spring Boot](https://img.shields.io/badge/Spring_Boot-F2F4F9?style=for-the-badge&logo=spring-boot)](https://spring.io/projects/spring-boot)

&nbsp; [![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=Swagger&logoColor=white)](https://swagger.io/)

&nbsp; [![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)](https://jwt.io/)

### Frontend

&nbsp; [![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)

&nbsp; [![Redux](https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white)](https://redux.js.org/)

&nbsp; [![MUI](https://img.shields.io/badge/Material%20UI-007FFF?style=for-the-badge&logo=mui&logoColor=white)](https://mui.com/material-ui/)

&nbsp; [![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

&nbsp; [![Axios](https://img.shields.io/badge/axios-671ddf?&style=for-the-badge&logo=axios&logoColor=white)](https://axios-http.com/)

&nbsp; [![Vite](https://img.shields.io/badge/Vite-B73BFE?style=for-the-badge&logo=vite&logoColor=FFD62E)](https://vitejs.dev/)

&nbsp; [![ESLint](https://img.shields.io/badge/ESLint-4B3263?style=for-the-badge&logo=eslint&logoColor=white)](https://eslint.org/)

&nbsp; ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)

&nbsp; [![.Env](https://img.shields.io/badge/.ENV-ECD53F.svg?style=for-the-badge&logo=dotenv&logoColor=black)](https://www.ibm.com/docs/bg/aix/7.2?topic=files-env-file)

&nbsp; ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)

### Test

&nbsp; [![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)](https://www.postman.com/)


<br/>

<h2 id="features">🔥 Features</h2>

### Configuration

+ **Auto-Renewal of Trusted TLS Certificates:** Automatic renewal of trusted TLS certificates to ensure uninterrupted security in production environments.
+ **Trusted TLS Certificates:** Secure communication between services using trusted SSL certificates managed by Traefik for production environment.
+ **Self-Signed TLS Certificates:** Secure communication between services using self-signed SSL certificates managed by Traefik for local development.
+ **Traefik Load Balancing:** Load balancing configured through Traefik for improved scalability and also local service development.
+ **Traefik Router:** Routing configured through Traefik for service communication without exposing port to public.
+ **Centralized TLS Security:** Centralized TLS certificate configuration across all services.
+ **Traefik Dashboard:** Dashboard integrated for monitoring and managing Traefik services, routers and prefixes.
+ **Traefik Integration:** Traefik integrated for networking.
+ **Docker-Compose Configuration:** Comprehensive Docker-Compose configuration for managing service orchestration.
+ **Docker Containerization:** The application is containerized for consistent deployment.

### Frontend

+ **Custom Modal:** Includes a custom modal component with configurable actions to enhance user interaction.
+ **TLS/HTTPS:** Centeralized TLS/HTTPS support for all services with selfsigned certificate.
+ **Traefik Integration:** Integration with Traefik for efficient load balancing and port forwarding within the application's microservices architecture.
+ **External Communication:** Manages communication between backend and email service.
+ **Global State Management:** Redux implementation for consistent state handling across the application.
+ **Persistent Settings:** Language, theme mode, and theme schema are stored in localStorage.
+ **Internationalization:** Language support with i18n for a multilingual user experience.
+ **Custom Scrollbar Design:** Unique scrollbar styling to match the application's aesthetic.
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
+ **Backend Integration:** Integration with the backend service.

### Backend

+ **TLS/HTTPS:** Centeralized TLS/HTTPS support for all services with selfsigned certificate.
+ **External Communication:** Manage communication with frontend.
+ **Postman Endpoint Collection:** Postman collection added for ensure validation of all API endpoints.
+ **Swagger Documentation:** Comprehensive API documentation integrated for documentation and testing purposes.
+ **Environment Configuration:** Configurations have been adjusted for enhanced flexibility.
+ **Dockerization:** The application is containerized for consistent deployment and scaling.

### Email Service

+ **TLS/HTTPS:** Centeralized TLS/HTTPS support for all services with selfsigned certificate.
+ **External Communication:** Manage communication with frontend.
+ **Postman Endpoint Collection:** Postman collection added for ensure validation of all API endpoints.
+ **Swagger Documentation:** Comprehensive API documentation integrated for documentation and testing purposes.
+ **Environment Configuration:** Configurations have been adjusted for enhanced flexibility.
+ **Dockerization:** The application is containerized for consistent deployment and scaling.

<br/>

<h2 id="releases">🚢 Releases</h2> 

&nbsp; [![.](https://img.shields.io/badge/v2-233838?style=flat&label=deploy&labelColor=470137&color=077521)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/deploy-v1)

&nbsp; [![.](https://img.shields.io/badge/v1-233838?style=flat&label=deploy&labelColor=470137&color=077521)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/deploy-v2)

&nbsp; [![.](https://img.shields.io/badge/3.0.1-233838?style=flat&label=release&labelColor=470137&color=077521)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/3.0.1)

&nbsp; [![.](https://img.shields.io/badge/3.0.0-233838?style=flat&label=release&labelColor=470137&color=077521)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/3.0.0)

&nbsp; [![.](https://img.shields.io/badge/2.0.0-233838?style=flat&label=release&labelColor=470137&color=077521)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/2.0.0)

&nbsp; [![.](https://img.shields.io/badge/1.1.0-233838?style=flat&label=release&labelColor=470137&color=077521)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/1.1.0)

&nbsp; [![.](https://img.shields.io/badge/1.0.0-233838?style=flat&label=release&labelColor=470137&color=077521)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/1.0.0)

<br/>

<h2 id="traefik-dashboard">🚥 Traefik Dashboard</h2> 
You can monitor and manage your services through the Traefik dashboard.

To view the dashboard visit: [`traefik`](https://traefik.localhost).

<img width=500 src="assets/traefik/traefikDashboard.png">

<br/>

<h2 id="system-links">🔗 System Links</h2> 

| Service            | URL                                                |
|--------------------|----------------------------------------------------|
| Frontend           | https://localhost/                                 |
| Traefik Dashboard  | https://localhost/traefik/dashboard/#/             |
| Backend Swagger UI | https://localhost/backend/sw/swagger-ui/index.html |
| Email Swagger UI   | https://localhost/email/sw/swagger-ui/index.html   |

<br/>

<h2 id="system-preperation">🔧 System Preperation</h2>

### Docker Config
#### Production
* Obtain a domain name.
* Update the domain name in the traefik-conf/docker-compose.yml file, replacing "localhost" with your domain.

<br/>

* Change permission of the `/crt/acme.json` file with `chmod 600` with deploy/v2.
  
or

* Obtain a certificate for your domain with deploy/v1.
* Place the key files into `/crt` folder.
* Update `docker-compose` and `traefik-conf/docker-compose.yml` files with key file names.


  
#### Development
* Generate a self-signed certificate using OpenSSL.
```
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout selfsigned.key -out selfsigned.crt
```
* Place `selfsignd.key` and `selfsigned.crt` file into `/crt` folder.

<br/>

### Frontend
* To change system configs revise .env file.
  
<br/>

### Backend
#### Production
* Copy `application-dev.properties` to create `application-prod.properties`.
* Change `app.var.appMode` to `prod`.
* Change `server.port` to `80`.

<br/>

### Email Service
#### Production
* Copy `application-dev.properties` to create `application-prod.properties`.
* Change `app.var.appMode` to `prod`.
* Change `server.port` to `80`.
* Place credentials.

#### Development
* Place credentials in the `application-dev.properties` file.

<br/>

<h2 id="system-startup">🚀 System Startup</h2> 

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

<br/>

<h2 id="contributors">👥 Contributors</h2> 

<a href="https://github.com/ahmettoguz" target="_blank"><img width=60 height=60 src="https://avatars.githubusercontent.com/u/101711642?v=4"></a> 

### [🔝](#top)
