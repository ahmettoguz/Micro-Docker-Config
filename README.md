<h1 id="top" align="center">🚢 Release Version 2.0.0 </h1> 

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
| Micro-Docker-Config   | [![.](https://img.shields.io/badge/2.0.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Docker-Config/tree/release/2.0.0)   |
| Micro-Backend         | [![.](https://img.shields.io/badge/1.2.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Backend/tree/release/1.2.0)         |
| Micro-Email-Service   | [![.](https://img.shields.io/badge/1.1.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Email-Service/tree/release/1.1.0)   |
| Micro-Frontend        | [![.](https://img.shields.io/badge/2.1.0-233838?style=flat&label=release&labelColor=4A154B&color=233838)](https://github.com/ahmettoguz/Micro-Frontend/tree/release/2.1.0)        |

<br/>

<h2 id="features">🔥 Features</h2>

### Frontend

+ **External Communication:** Manages interaction between backend and email service.
+ **Global State Management:** Implemented using Redux for consistent state handling across the application.
+ **Persistent Settings:** Language, theme mode, and theme schema are remembered using localStorage.
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
+ **Docker Containerization:** The application has been containerized using Docker.
+ **Backend Integration:** Integration with the backend is complete.

### Backend

+ **External Communication:** Manage communication with frontend.
+ **Swagger Documentation:** Comprehensive API documentation integrated for easier development.
+ **Environment Variables:** Configurations have been adjusted for enhanced flexibility.
+ **Dockerized Application:** The application is containerized for consistent deployment and scaling.


### Email Service

+ **External Frontend Communication:** Seamlessly integrates with external frontends.
+ **Manual Testing:** Postman used for endpoint testing.
+ **Swagger Documentation:** API documentation integrated for streamlined development.
+ **Environment Configuration:** Variables have been adjusted for optimal flexibility.
+ **Dockerization:** The application is containerized for consistent deployment.
  
<br/>

<h2 id="next-release-features">🚧 Next Release Features</h2>

### Frontend
- Internal communication between backend service.
- TLS/HTTPS support.

### Backend
- TLS/HTTPS support.

### Email Service
- Service availability.

<br/>
  
<h2 id="system-startup">🚀 System Startup</h2> 

```
docker-compose -p micro up -d --build

docker-compose -p micro down

docker-compose ls
```

[🔝](#top)
