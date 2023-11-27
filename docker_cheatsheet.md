| Command | Description | Example |
|---|---|---|
| docker ps | Lists all running containers | docker ps |
| docker ps -a | Lists all containers, including stopped and exited containers | docker ps -a |
| docker images | Lists all images | docker images |
| docker pull <image-name> | Pulls an image from Docker Hub | docker pull nginx:latest |
| docker run <image-name> | Runs an image as a container | docker run nginx:latest |
| docker stop <container-id> | Stops a running container | docker stop <container-id> |
| docker rm <container-id> | Removes a stopped container | docker rm <container-id> |
| docker build -t <image-name> . | Builds an image from the current directory | docker build -t my-image:latest . |
| docker commit <container-id> <image-name> | Commits a running container to an image | docker commit <container-id> my-image:latest |
| docker exec -it <container-id> <command> | Executes a command in a running container | docker exec -it <container-id> bash |
| docker logs <container-id> | Prints the logs of a container | docker logs <container-id> |

**Examples:**

* To start an Nginx web server container, use the following command:

```bash
docker run -d -p 80:80 nginx:latest
```

This command will pull the Nginx image from Docker Hub if it is not already present, and then run it as a container. The `-d` flag tells Docker to run the container in the background, and the `-p 80:80` flag tells Docker to map port 80 on the host machine to port 80 on the container.

* To build an image from the current directory, use the following command:

```bash
docker build -t my-image:latest .
```

This command will build an image named `my-image:latest` from the Dockerfile in the current directory.

* To execute a command in a running container, use the following command:

```bash
docker exec -it <container-id> bash
```

This command will open a bash shell in the container with the specified ID.


