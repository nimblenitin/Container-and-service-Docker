# Container-and-service-Docker

Steps to-
    • Run a container from an image 
    • Run the image as a replicated service
    
```

1. List all the nodes in the swarm cluster
$ docker node ls

2. Pull the nginx image from Docker Hub
$ docker pull nginx:latest

3. Run a container from the nginx image
$ docker container run -d --name nginx-container nginx:latest

4. Find all the running containers
$ docker ps

5.Run the nginx image as a service
$ docker service create --name nginx-service --replicas 4 nginx:latest

6. Find all the services running in the swarm
$ docker service ls

7. List all the tasks of the nginx-service
$ docker service ps nginx-service


```
