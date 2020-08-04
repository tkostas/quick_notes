# Docker - Notes

* `docker login <repository url>`: Login to an container image repository.
* `docker build -t <image name:tag> .`: Build image
* `docker push <image name:tag>`: Push to container repository.
* `docker rmi <image name:tag>`: Remove image.
* `docker rm $(docker ps -a -q)`: Remove stopped containers.
* `docker run --env-file env -p <port-out>:<port-in> <image-name> <cmd>`: Run an container providing an `env` file and port.
