# Tour-Agency-Spring-Boot-Microservices
Creating RESTful Spring Boot microservices for a California-based tour agency using Spring Data, Spring MVC, Docker, Spring Security, and Spring Cloud.

Three microservices - 
1. explorecali-gateway : Gateway to below two microservices
2. explorecali-images : To upload images of tour
3. explorecali-jpa : To manage and retrieve details such as tour, tourpackage and tour ratings.

Each microservice is a project inside this main project 'Tour-Agency-Spring-Boot-Microservices'. Run individual microservice by navigating to its own directory. Use Github codespaces for running microservices online on Github platform. Add 'Spring Dashboard' and 'Docker' extensions in codespaces. 

Commands to run microservice - 
1. mvn clean complile -DskipTests
2. Go to Spring Dashboard and click play button on app.
3. Go to Docker Dashboard for docker containers.
4. Application will start running on 'http://{codespace-URL}/swagger-ui/index.html"
   For e.g. - https://effective-space-doodle-jq59g97w4562q44x-8080.app.github.dev/swagger-ui/index.html#/
