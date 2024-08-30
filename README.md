<h1 id="top" align="center">🚢 Release Version 3.0.0 </h1> 

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
| Micro-Docker-Config   | [![.](https://img.shields.io/badge/3.0.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/3.0.0)   |
| Micro-Backend         | [![.](https://img.shields.io/badge/1.2.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Backend/tree/release/1.2.0)         |
| Micro-Email-Service   | [![.](https://img.shields.io/badge/1.1.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Email-Service/tree/release/1.1.0)   |
| Micro-Frontend        | [![.](https://img.shields.io/badge/2.2.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Frontend/tree/release/2.2.0)        |

<br/>

<h2 id="features">🔥 Features</h2>

### Frontend

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
+ **Docker Containerization:** The application is containerized for consistent deployment.
+ **Backend Integration:** Integration with the backend service.

### Backend

+ **External Communication:** Manage communication with frontend.
+ **Swagger Documentation:** Endpoint documentation integrated for documentation and testing purposes.
+ **Environment Variables:** Configurations have been adjusted for enhanced flexibility.
+ **Dockerized Application:** The application is containerized for consistent deployment.


### Email Service

+ **External Communication:** Manage communication with frontend.
+ **Manual Testing:** Postman used for endpoint testing.
+ **Swagger Documentation:** Endpoint documentation integrated for documentation and testing purposes.
+ **Environment Configuration:** Configurations have been adjusted for enhanced flexibility.
+ **Dockerization:** The application is containerized for consistent deployment.
  
<br/>

<h2 id="next-release-features">🚧 Next Release Features</h2>

### Frontend
- Animated counter
- Scroll reveal

### Backend
- Postman requests


### Email Service
- Authentication

  
<br/>
  
<h2 id="system-startup">🚀 System Startup</h2> 

```
docker-compose -p micro up -d --build

docker-compose -p micro down

docker-compose -p micro up -d reverse-proxy --build

docker-compose -p micro down reverse-proxy

docker-compose ls
```

### [🔝](#top)
