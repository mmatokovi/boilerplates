### Installation with Docker

🛳️ Docker templates and boilerplates for various projects 

Make sure you have [Docker](https://www.docker.com/)

Exploring Docker container's file system
Docker version 1.3 or newer supports the command exec that behave similar to nsenter. This command can run new process in already running container (container must have PID 1 process running already). You can run /bin/bash to explore container state:

`docker exec -t -i mycontainer /bin/bash`
see Docker command line documentation