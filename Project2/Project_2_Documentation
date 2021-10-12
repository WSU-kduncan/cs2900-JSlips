# Project 2: Working with Containers

**Here's a quick quiz**
True or False
1. Did I get my wisdom teeth removed earlier today and I'm just now working on a project that has been announced for nearly a month?
Take a wild shot at the answer to this one :)

## Container Technologies 
1. Podman
2. Docker (Not Docker Desktop)

## Installation on Kali Linux

### How to Install Podman
1. First off, navigate to your systems terminal / command prompt. 
2. Optionally, run this command `sudo apt-get -y update` to update your apt-get tool.
3. To install Podman, simply run `sudo apt-get -y install podman`.
4. Podman should now run through an installation process and be installed on your system.

### How to Install Docker
1. First off, navigate to your systems terminal / command prompt.
2. Optionally, run this command `apt-get update` to update your apt-get tool.
3. Use the following command to install and setup the docker repo. `sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release`
4. You will also need to add dockers official gpg key. ` curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg`
5. After the docker repo is setup, we can run `sudo apt-get update` AND `sudo apt-get install docker-ce docker-ce-cli containerd.io` to install Docker Engine.

## Pulling a container image

### Podman: 
1. In order to pull an image with podman, use the command `podman pull [source]` where source is the source of the image.
In this case, I used 'ubuntu' as my image source. `Ubuntu` is an alias.
2. You should recieve a hash if all went well and you should also be able to view your images using `podman images`.

### Docker:
1. In order to pull an image with docker, use the command `docker pull [source]` where source is the source of the image.
I used `ubuntu` as my source in this case. Ubuntu is an alias.
2. You should be able to view your pulled images using `docker images`

## Running a Container

### Podman:
Podman can be run in various different modes.
1. Running Podman in shell mode us quite easy. The syntax to run in shell mode is `podman run [options] image [args]`, where image is required. 
2. Podman can run in detached mode by using the `--deatch` or `-d` argument. This will have the container run in the background and print the new container ID. 
3. Initializing a container and running the container are indeed two different things. Initalizing a container conducts the tasks needed for starting the countainer (such as mounting file systems and initalizing the network) however it does NOT start the container. 
4. If you do not initiazlize a container, it will do so automatically while using any of the run commands mentioned above. 

### Docker:
1. You can run docker in shell mode quite easily. Use the command `docker exec [OPTIONS] CONTAINER COMMAND [ARG...]`
2. If you want to run docker in detached mode, you can use `--detach` OR `-d`. Running in detached mode allows the command to be run in the background.
3. Initializing a container and running the container are indeed two different things. Initalizing a container conducts the tasks needed for starting the countainer (such as mounting file systems and initalizing the network) however it does NOT start the container. 
4. If you do not initiazlize a container, it will do so automatically while using any of the run commands mentioned above. 


## Logs and Status

## Podman: 
1. There are many reasons why you would want to view the status of the container. The syntax to view the status of the container is `podman ps [options]`. This command will show information such as container id, name of image, the time created, status of container, and more!
2. To view logs, use the log command `podman logs [options] container [container...]`. This command will provide the logs present for one or more containers specified.

### Docker:
1. To view the status of your containers, we actually do not use the `status` command. This is a depreciated command used for viewing the status of the docker installation. In order to view the container status, we can use `docker compose ps [SERVICE...]`
2. To view the logs of docker, we can use the `docker logs [OPTIONS] CONTAINER`. This command will retrieve the logs present for docker at the time of execution. Use the `--details` arguement to show extra details provided to logs.

## Stopping a container:

### Podman: 
1. In order to stop a container, simply run the `podman stop [options] container` command. This stops the specified container. This command takes the container ID or name as input. 
2. In order to pause a container, simply run the `podman pause [options] container` command. This pauses all processes in the specified containers. 
3. In order to restart a container, simply run the `podman restart [options] container`. This command will restart all containers specified. 

## Docker:
1. In order to stop a container, simply run the `docker compose stop [options] [SERVICE...]` command. This stops the specified container. This command takes the container ID or name as input. 
2. In order to pause a container, simply run the `docker compose pause [SERVICE...]` command. This pauses all processes in the specified containers. Use `docker compose unpause` to unpause.
3. In order to restart a container, simply run the `docker compose restart [options] [SERVICE...]`. This command will restart all containers specified. 

##

