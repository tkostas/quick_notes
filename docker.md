# Docker - Notes

* `docker login <repository url>`: Login to an container image repository.
* `docker build -t <image name:tag> .`: Build image
* `docker push <image name:tag>`: Push to container repository.
* `docker rmi <image name:tag>`: Remove image.
* `docker rm $(docker ps -a -q)`: Remove stopped containers.
* `docker run --env-file env -p <port-out>:<port-in> <image-name> <cmd>`: Run an container providing an `env` file and port. (https://docs.docker.com/engine/reference/commandline/run/)
* `docker ps`: List containers (https://docs.docker.com/engine/reference/commandline/ps/)
* `docker exec <image name> <command>`: e.g. `docker exec webapp:v1.0.0 bash`
