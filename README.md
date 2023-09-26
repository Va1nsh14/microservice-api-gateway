# Microservice API Gateway
Using Java 8 and Spring Eureka

### How to create databases in local env
(Prerequisites: Install Docker in your local enviroment)

- Use following commands to run and open shell from that `mongodb-commiunity-server` docker image
```
export MONGODB_VERSION=6.0-ubi8
docker run --name mongodb -d -p 64000:27017 mongodb/mongodb-community-server:$MONGODB_VERSION
docker exec -it $(docker ps --filter "name=mongodb" --format "{{.ID}}") sh
```