Joey Carusone - Project 3

## Part 1: Investigate available mounts

1. **Docker-** uses volumes and bind mounts. 
	__Bind mounts__ are stored anywhere on the host filesystem and is mounted into a running container from an existing file or folder. Since bind mounts can exist anywhere, any process is able to modify it (even outside of Docker).
	__Volumes__  are the recommended way to store data in the docker universe due to them being completely managed by Docker.
	
	**Podman-** uses bind mounts, volumes, images, and tmpfs.
	__Bind mounts__ work the same way in podman compared to docker.
	__Volumes__ are created in podman using `podman volume create` and have the same effect in podman compared to docker. 
	__Images__ mount type mounts the specified images' root filesystem in a place that the host can access. It then returns the location back.
	__Tmpfs__ and the content within them are temporary and go away when the container is stopped. 
	
## Part 2: Investigate building images for the container engine.

2. **Docker-** uses Dockerfiles to build images.
	You can build an image in Docker by using `docker build [OPTIONS] PATH | URL |`
	You can write a dockerfile by using FROM, COPY, RUN, and CMD. 
	
	FROM: creates later from ubuntu:18.04 Docker image.
	COPY: adds files from Docker to current directory.
	RUN: builds applications using `make`
	CMD: used to specify what command to run within container.
	
	**Podman-** uses Containerfiles to build images.
	You can build an image in Podman by using `podman build [options] [context]`
	You can write a containerfile by using the same syntax as a dockerfile. In fact, your containerfile can also be named dockerfile due to such similar syntax. 
	
	Buildah can be used as the image builder, but Podman supports how the method to create Dockerfiles: 
	
	FROM: creates later from ubuntu:18.04 Docker image.
	COPY: adds files from Docker to current directory.
	RUN: builds applications using `make`
	CMD: used to specify what command to run within container.

