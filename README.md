# 📦 Docker Command Reference  

## 📖 Introduction to Docker  
Docker is a platform designed to make it easier to develop, deploy, and run applications by using containers. Containers are lightweight, portable, and ensure consistency across various environments.  

This guide provides a categorized list of Docker commands to help you manage containers, images, networks, and more efficiently.  

---

## 🛠️ Common Docker Commands  
These are frequently used commands for everyday Docker operations:  

| Command           | Description                                                 |  
|-------------------|-------------------------------------------------------------|  
| `docker run`      | Create and run a new container from an image.               |  
| `docker exec`     | Execute a command in a running container.                   |  
| `docker ps`       | List running containers.                                    |  
| `docker build`    | Build an image from a Dockerfile.                           |  
| `docker pull`     | Download an image from a registry.                          |  
| `docker push`     | Upload an image to a registry.                              |  
| `docker images`   | List images stored locally.                                 |  
| `docker login`    | Authenticate to a registry.                                 |  
| `docker logout`   | Log out from a registry.                                    |  
| `docker search`   | Search Docker Hub for images.                               |  
| `docker version`  | Show the Docker version information.                        |  
| `docker info`     | Display system-wide information.                            |  
| `docker run -it`  | Start a new container interactively.                        |
| `docker run-d`    | Run container in the background.                            |
|`docker run -it bash`  | Run container and access it.                            |
|`docker run..sleep 20` | Run container for 20sec.                                | 
|`docker exec .. cat..` | Run command inside a running contianer.                 |
---

## 🔧 Management Commands  
Use these commands to manage different Docker components:  

| Command             | Description                                               |  
|---------------------|-----------------------------------------------------------|  
| `docker container`  | Manage containers.                                        |  
| `docker image`      | Manage images.                                            |  
| `docker network`    | Manage networks.                                          |  
| `docker volume`     | Manage volumes.                                           |  
| `docker system`     | Manage Docker resources.                                  |  
| `docker builder`    | Manage builds.                                            |  
| `docker compose`    | Use Docker Compose for multi-container applications.      |  

---

## ⚙️ Swarm Commands  
Manage Docker Swarm, Docker’s native clustering and orchestration tool:  

| Command      | Description                                                     |  
|--------------|-----------------------------------------------------------------|  
| `docker swarm` | Manage Swarm.                                                 |  

---

## 📂 Additional Commands  
These commands offer advanced features for working with containers and images:  

| Command           | Description                                                 |  
|-------------------|-------------------------------------------------------------|  
| `docker attach`   | Attach to a running container.                              |  
| `docker commit`   | Create a new image from a container’s changes.              |  
| `docker cp`       | Copy files/folders between a container and the local system.|  
| `docker create`   | Create a new container without starting it.                 |  
| `docker diff`     | Inspect changes to a container’s filesystem.                |  
| `docker events`   | Get real-time events from the Docker server.                |  
| `docker export`   | Export a container’s filesystem as a tar archive.           |  
| `docker history`  | Show the history of an image.                               |  
| `docker import`   | Import a tarball to create a filesystem image.              |  
| `docker inspect`  | Return detailed information on Docker objects.              |  
| `docker kill`     | Kill running containers.                                    |  
| `docker logs`     | Fetch the logs of a container.                              |  
| `docker pause`    | Pause all processes in a container.                         |  
| `docker restart`  | Restart a container.                                        |  
| `docker rm`       | Remove one or more containers.                              |  
| `docker rmi`      | Remove one or more images.                                  |  
| `docker stats`    | Display a live stream of container resource usage.          |  
| `docker stop`     | Stop a running container.                                   |  
| `docker tag`      | Create a new tag for an image.                              |  
| `docker update`   | Update configuration of one or more containers.             |  
| `docker wait`     | Block until a container stops, then print its exit code.    |  
| `docker start`    | Start and existing container                                |
---

## 📘 Additional Resources  
- [Docker Documentation](https://docs.docker.com)  
- [Docker Hub](https://hub.docker.com)  

---
