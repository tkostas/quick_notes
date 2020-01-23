# Docker - Notes

* `docker login <repository url>`: Login to an container image repository.
* `docker build -t <image name:tag> .`: Build image
* `docker push <image name:tag>`: Push to container repository.
* `docker rmi <image name:tag>`: Remove image.
* `docker rm $(docker ps -a -q)`: Remove stopped containers.
