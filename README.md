CRUD REST CALLS WITH REDIS DOCKER AND JWT
  
  docker build -t crud-nodejs-app .
  docker run -d -p 27017:27017 --name enggadda mongo:latest
  docker run -p 3000:3000 --name crud-nodejs-app --link enggadda:mongo -d crud-nodejs-app:latest
   http://localhost:8080/swagger-ui.html (or /swagger-ui/index.html)
