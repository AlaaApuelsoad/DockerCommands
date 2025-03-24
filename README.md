# Docker Command Reference

## Introduction to Docker  
Docker is a platform designed to make it easier to develop, deploy, and run applications using containers. Containers are lightweight, portable, and ensure consistency across various environments.

This guide provides a categorized list of Docker commands to help you efficiently manage containers, images, networks, and more.

---

## Common Docker Commands  
These are frequently used commands for everyday Docker operations:  

| Command                        | Description                                                 |  
|--------------------------------|-------------------------------------------------------------|  
| `docker version`               | Show the Docker version information.                        |  
| `docker info`                  | Display system-wide information.                            |  
| `docker login`                 | Authenticate to a registry.                                 |  
| `docker logout`                | Log out from a registry.                                    |  
| `docker search <image>`        | Search Docker Hub for images.                              |  
| `docker pull <image>`          | Download an image from a registry.                         |  
| `docker push <image>`          | Upload an image to a registry.                             |  

---

## Image Management Commands  
These commands help in handling Docker images:  

| Command                        | Description                                                 |  
|--------------------------------|-------------------------------------------------------------|  
| `docker images`                | List images stored locally.                                 |  
| `docker build -t <image>`      | Build an image from a Dockerfile.                          |  
| `docker tag <image> <tag>`     | Create a new tag for an image.                             |  
| `docker rmi <image>`           | Remove one or more images.                                 |  
| `docker rmi -f $(docker images -q)`  | Remove all images.                                   |  
| `docker history <image>`       | Show the history of an image.                              |  
| `docker inspect <image>`       | Return detailed information about an image.                |  

---

## Container Management Commands  
Manage Docker containers using these commands:  

| Command                         | Description                                                 |  
|---------------------------------|-------------------------------------------------------------|  
| `docker run <image>`            | Create and run a new container from an image.               |  
| `docker run -it <image>`        | Start a new container interactively.                        |  
| `docker run -d <image>`         | Run a container in the background.                          |  
| `docker run -it <image> bash`   | Run a container and access it.                              |  
| `docker run <image> sleep 20`   | Run a container for 20 seconds.                             |  
| `docker ps`                     | List running containers.                                    |  
| `docker ps -a`                  | List all containers (running & stopped).                    |  
| `docker exec -it <container> <cmd>` | Run a command inside a running container.             |  
| `docker start <container>`      | Start an existing container.                                |  
| `docker stop <container>`       | Stop a running container.                                   |  
| `docker restart <container>`    | Restart a container.                                        |  
| `docker kill <container>`       | Kill running containers.                                    |  
| `docker attach <container>`     | Attach to a running container.                              |  
| `docker logs <container>`       | Fetch the logs of a container.                              |  
| `docker pause <container>`      | Pause all processes in a container.                         |  
| `docker wait <container>`       | Block until a container stops, then print its exit code.    |  
| `docker rm <container>`         | Remove one or more containers.                              |  
| `docker stop $(docker ps -q)`   | Stop all running Docker containers.                         |  
| `docker rm $(docker ps -aq)`    | Delete all containers.                                      |  
| `docker create <image>`         | Create a new container without starting it.                 |  
| `docker commit <container> <new_image>` | Create a new image from a container's changes.    |  

---

## Network Management Commands  
Manage Docker networks with these commands:  

| Command                          | Description                                                 |  
|----------------------------------|-------------------------------------------------------------|  
| `docker network ls`              | List available networks.                                   |  
| `docker network create <name>`   | Create a new network.                                     |  
| `docker network inspect <name>`  | Inspect network details.                                  |  
| `docker network connect <net> <container>` | Connect a container to a network.              |  
| `docker network disconnect <net> <container>` | Disconnect a container from a network.       |  
| `docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' <container>` | Get the IP address of a container. |  

---

## Volume Management Commands  
Manage Docker volumes using these commands:  

| Command                          | Description                                                 |  
|----------------------------------|-------------------------------------------------------------|  
| `docker volume ls`               | List available volumes.                                    |  
| `docker volume create <name>`    | Create a new volume.                                      |  
| `docker volume inspect <name>`   | Get details of a volume.                                  |  
| `docker volume rm <name>`        | Remove a volume.                                          |  

---

## System Management Commands  
These commands help manage system-wide Docker resources:  

| Command                          | Description                                                 |  
|----------------------------------|-------------------------------------------------------------|  
| `docker system df`               | Show Docker disk usage.                                    |  
| `docker system prune`            | Remove unused data (containers, images, networks, etc.).  |  

---

## Docker Compose Commands  
Manage multi-container applications using Docker Compose:  

| Command                          | Description                                                 |  
|----------------------------------|-------------------------------------------------------------|  
| `docker-compose up -d`           | Start containers in detached mode.                         |  
| `docker-compose down`            | Stop and remove containers.                               |  
| `docker-compose ps`              | List running services.                                    |  
| `docker-compose exec <service> <cmd>` | Run a command inside a service container.         |  

---

## Swarm Commands  
Manage Docker Swarm (native clustering and orchestration tool):  

| Command                          | Description                                                 |  
|----------------------------------|-------------------------------------------------------------|  
| `docker swarm init`              | Initialize a new Swarm.                                    |  
| `docker swarm join <args>`       | Join an existing Swarm.                                   |  
| `docker swarm leave`             | Leave the Swarm cluster.                                  |  

---

## File Management Commands inside a Container  
These commands help list and access files inside a running Docker container:

| Command                                      | Description                                      |
|---------------------------------------------|------------------------------------------------|
| `docker exec -it <container> ls /path`      | List files in a specific directory.            |
| `docker exec -it <container> find / -name "<file>"` | Search for a file inside the container.  |
| `docker exec -it <container> cat /path/file` | View the content of a file.                    |
| `docker exec -it <container> more /path/file` | View file content page by page.                |
| `docker exec -it <container> less /path/file` | Scroll through a file's content.               |
| `docker exec -it <container> vi /path/file`  | Open a file with the `vi` editor.              |

## Additional Resources  
- [Docker Documentation](https://docs.docker.com)  
- [Docker Hub](https://hub.docker.com)  
