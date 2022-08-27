# inventory-management
Software de manejo de inventario diseñado en una arquitectura de microservicios con spring boot y springcloud, autenticación y autorización con Spring Cloud Security (OAuth2 y JWT), balanceo de carga del lado del cliente con Spring Cloud LoadBalancer y Ribbon, tolerancia a fallos y latencia con Resilience4J y Hystrix, rastreo distribuido en microservicios con Spring Cloud Sleuth y Zipkin 

### Iniciar la aplicación 
Asegurarse de tener
Java 11 + 
Postman

### Agregar la configuración de la base en applicacitons.properties 
Este paso es necesario

Importar el script de la base de datos en el motor de bases de datos mysql

/src/main/resources/application.properties

Actualiza las siguientes propiedades 

* url 
* username 
* password

#### Ejecutalo
Usar intellij IDEA para abrir el proyecto, tutorial con los pasos necesarios: https://medium.com/backend-habit/intellij-idea-running-multiple-project-microservices-in-one-workspace-d61126fe0eef
Ejecutar cada uno de los proyectos maven, orden: 1- SpringBootServicioConfigServerApplication 2- SpringBootServicioEurekaServerApplication 3- SpringBootServicioZuulServerApplication 4- SpringBootServicioOauthServerApplication 5- SpringBootServicioUsuariosServerApplication 6- SpringBootServicioProductosServerApplication

Enviar el request en el archivo postman adjunto para generar el token de autenticación
![image](https://user-images.githubusercontent.com/60546141/187045184-c1676510-6eaa-46e7-a03f-f161d7ea6422.png)
Agregar la cabecera bearer token y en el campo ingresar el token generado, luego probar las apis de la aplicación
![image](https://user-images.githubusercontent.com/60546141/187045235-0fbc68bd-32ad-4d5d-bce7-5e7ae262f6d4.png)


## Authors ✒️

* **Deiby Castaño** - *Desarrollo y documentacion* - [deibyalejandro](https://github.com/deibyalejandro)

Etapa práctica del curso de microservicios con spring boot y spring cloud [Udemy](https://www.udemy.com/course/microservicios-con-spring-boot-y-spring-cloud/)
