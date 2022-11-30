| Command | Description | Note | Version | Docs |
|:--- |:--- |:--- |:--- |:--- |
| `docker attach <container_id>` | attach to the container's terminal  | | |
| `docker build <directory_path> -t <image_name>` | build tagged container image localy on the system | directory must contain a `Dockerfile` | |
| `docker container stop <container_name>` | stop container | | |
| `docker exec -it <container_name> <command>` |  start command inside a container in terminal interactive mode | | |
| `docker exec <container_name> <command>` | start command inside a container | | |
| `docker history <image_name>` | display layers of the container image with their sizes | | |
| `docker images` | list all of the images and their sizes | | |
| `docker images -f "dangling=true"` | list all dangling images | | |
| `docker info` | show basic information about docker configuration | | |
| `docker inspect <image_name>` | display detailed information about the container | | |
| `docker logs <container_id>` | displey container logs | | |
| `docker ps -a` | list all docker containers | lists stopped ones also | |
| `docker pull <image_name:tag>` | pull docker image from the docker repository | | |
| `docker pull <image_name>` | pull docker image and store it on the host machine | | |
| `docker push <image_name>` | push container to the docker repository | | |
| `docker rmi $(docker images -f "dangling=true" -q --no-trunc)` | remove dangling images only | | |
| `docker rmi <image_id>` | remove docker image permanently | | |
| `docker run --cpus=<value> <image_name>` | run container with restricted cpu utilization | | |
| `docker run --entry_point <command> <image_name> <parameters>` | | | |
| `docker run --memory=<value> <image_name>` | run container with restricted memory utilization | | |
| `docker run -d <iamge_name>` | run container in the background | | |
| `docker run -e <variable_name>=<value> <image_name>` | set the value for the variable of the container | | |
| `docker run -it <image_name>` | run container in the interactive mode while attached to the terminal | | |
| `docker run -p <localhost_port>:<container_port> <image_name>` | mapping the localhost port to the container port | | |
| `docker run -v <host_directory_path>:<container_path>  <image_name>` | run container with mounted host directory to the container | | |
| `docker run -v <host_path>:<container_path> <image_name>` | volume mapping; map host directory to the directory inside the container | | |
| `docker run -v <volume_name>:<container_path> <image_name>` | run container with mounted volume | creates volume directory if it does not exist | |
| `docker run <image_name>` | run docker container | | |
| `docker run <image_name> <command>` | run container by invoking specific commmand | | |
| `docker run <image_name>:<tag>` | run specific version of the docker container | | |
| `docker stop ```docker ps -q``` ` | stop all the containers | | |
| `docker stop <container_id>` | | | |
| `docker system prune` | remove stopped containers, dangling images, dangling build cache | | |
| `docker volume create <volume_name>` | create docker persistance directory | | |
| `docker volume inspect <volume_name>` | inspect a volume | | |
| `docker volume ls` | list all volumes | | |
| `docker volume prune` | remove all volumes | | |
| `docker volume rm <volume_name>` | remove a volume | | |
| `docker-compose up` | | | |
