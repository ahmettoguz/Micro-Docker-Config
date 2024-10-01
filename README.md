<h1 id="top" align="center">🚢 Release Version 3.1.0 </h1> 

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
| Micro-Docker-Config   | [![.](https://img.shields.io/badge/3.0.1-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/3.0.1)   |
| Micro-Backend         | [![.](https://img.shields.io/badge/1.2.1-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Backend/tree/release/1.2.1)         |
| Micro-Email-Service   | [![.](https://img.shields.io/badge/1.1.2-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Email-Service/tree/release/1.1.2)   |
| Micro-Frontend        | [![.](https://img.shields.io/badge/2.3.1-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Frontend/tree/release/2.3.1)        |

<br/>

<h2 id="features">🔥 Features</h2>

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

<h2 id="next-release-features">🚧 Next Release Features</h2>

### Frontend
- Animated counter
- Scroll reveal

<br/>

<h2 id="system-links">🔗 System Links</h2> 

| Service            | URL                                                        |
|--------------------|------------------------------------------------------------|
| Frontend           | https://sendpshere.com.tr/                                 |
| Traefik Dashboard  | https://sendpshere.com.tr/traefik/dashboard/#/             |
| Backend Swagger UI | https://sendpshere.com.tr/backend/sw/swagger-ui/index.html |
| Email Swagger UI   | https://sendpshere.com.tr/email/sw/swagger-ui/index.html   |

<br/>

<h2 id="system-preperation">🔧 System Preperation</h2>


### Docker Config
#### Production
* Obtain a domain name.
* Update the domain name in the traefik-conf/traefik-dynamic.yml file, replacing current domain name with your domain.
* Place email address to traefik-conf/treafik.yml
* Change permission of the `/crt/acme.json` file with `chmod 600` with deploy/v2.
  
or

* Obtain a domain name.
* Obtain a certificate for your domain with deploy/v1.
* Place the key files into `/crt` folder.
* Update `docker-compose` and `traefik-conf/docker-compose.yml` files with key file names.

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
* Go to your Google Account settings at [`myaccount.google.com`](https://myaccount.google.com/).
* In the navigation panel, select [`Security`](https://myaccount.google.com/security).
* Under `How you sign in to Google`, select `2-Step Verification`.
* Add your phone number as a verification method.
* Go to  [`myaccount.google.com/u/1/apppasswords`](https://myaccount.google.com/u/1/apppasswords) and generate a new app password.
* Copy `application-dev.properties` to create `application-prod.properties`.
* Change `app.var.appMode` to `prod`.
* Change `server.port` to `80`.
* Place credentials.

#### Development
* Place credentials in the `application-dev.properties` file.

<br/>
  
<h2 id="system-startup">🚀 System Startup</h2>

```
docker compose -p micro down
docker compose -p micro up -d --build

docker compose -p micro down reverse-proxy
docker compose -p micro up -d reverse-proxy --build

docker compose -p micro down frontend
docker compose -p micro up -d frontend --build

docker compose -p micro down backend
docker compose -p micro up -d backend --build

docker compose -p micro down email-service
docker compose -p micro up -d email-service --build

docker compose ls
```

### [🔝](#top)
