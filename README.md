# Tour-Agency-Spring-Boot-Microservices
Creating RESTful Spring Boot microservices for a California-based tour agency using Spring Data, Spring MVC, Docker, Spring Security, and Spring Cloud.

Three microservices - 
1. explorecali-gateway : Spring Cloud Gateway microservice to route requests to below two microservices
2. explorecali-images : Spring RESTful microservice to upload and store images of tours to MongoDB database.
3. explorecali-jpa : Spring RESTful microservice to manage and retrieve details such as tours, tour packages, and tour ratings from a MySQL database.

Each microservice is a project inside this main project 'Tour-Agency-Spring-Boot-Microservices'. Run individual microservice by navigating to its own directory or run all three in dockerized containers with a single command using docker-compose. Use Github codespaces for running microservices online on Github platform. Add 'Spring Dashboard' and 'Docker' extensions in codespaces. 

Running individually - 
1. Run microservice by navigating to its directory : mvn clean compile -DskipTests spring-boot:run
3. Go to Spring Dashboard and view microservice is up and running.
4. Go to Docker Dashboard to view docker containers.
5. View and run APIs on Swagger UI running on 'http://{codespace-URL}/swagger-ui/index.html'
   For e.g. - https://effective-space-doodle-jq59g97w4562q44x-8080.app.github.dev/swagger-ui/index.html#/
6. Since microservice is running on codespace (and not locally), Postman cannot be used to run APIs.
   Use curl (commands available in curlcommands.txt) to interact with APIs

Running whole application - 
1. Running all three microservices with a single command : mvn clean compile jib:dockerBuild && docker-compose up
2. Open another terminal and execute command to verify : curl -v localhost:8080/packages
3. More commands available in curlcommands.tx
