# Installation with Docker

🛳️ Docker templates and boilerplates for various projects

Make sure you have [Docker](https://www.docker.com/) and running

Exploring Docker container's file system
Docker version 1.3 or newer supports the command exec that behave similar to nsenter. This command can run new process in already running container (container must have PID 1 process running already).  
You can run /bin/bash to explore container state:

## Commands

`docker container ls` - List all container imgs

`docker container run -p` - exposes port on machine

`docker container inspect --format '{{ .NetworkSettings.IPAddress }}' webhost` - show ip address of container

`docker network inspect {bridge_network}` - show network info

### Getting a Shell Inside Containers

`docker container run -it` - start new container interactively

`docker container exec -it` - run additional command in existing container

`ls -al` - look all files inside of container