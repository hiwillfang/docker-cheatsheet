# DOCKER CHEATSHEET
This is a list of commonly used [Docker](https://www.docker.com/) commands for any "Dockerized" app development workflow for developers.

### What's Docker and why use it?
Docker is the world's leading software container platform. Developers use Docker to eliminate the "works on my machine" problems when collaborating on code. Regardless if your OS is Mac, Windows, or a Linux Distro, Docker apps are completely portable and platform agnostic. Docker also manages and tracks changes and dependencies, which makes it easier for sysadmins to understand how the apps works.

### Key Features
* Compose file to deploy Swarm mode services
* Improved CLI backwards compatibility
* Clean-up commands
* CLI Restructure
* Monitoring and build improvements

### Docker Version 1.13
As of the latest version (1.13) of Docker, Docker has reorganized it's commands into **management commands** and **sub-commands**. To see a list of all Docker commands run `docker`. This change is primarily associated with simplifying the CLI structure. All old commands will still work due to Docker's backwards compatibility.

**DOCKER COMMAND FORMAT:**
`docker <command> <sub-command> (options)`

* Get information on the latest version of Docker installed on your machine:

	`docker version`

* Get Docker stats like how many containers and images are running:

	`docker info`

* Print a list of all commands provided by Docker:

	`docker`

* Manage Docker volumes:

	`docker volume`

* Block until a container stops, then print its exit code:

	`docker container wait`

* Display all images: 

	`docker images`

* List your running containers:

	`docker container ls`

	`docker container ls -a (-a flag lists all containers running or not)`

* Start one or more running containers:

	`docker container start`

* Stop one or more running containers:

	`docker container stop`

* Display logs for a specific container:

	`docker container logs container_name`

	To see all log options:

	`docker container logs --help`

* List running processes in a specific container:

	`docker top container_id`

* Unpause all processes within one or more containers:

	`docker container unpause`

* Display metadata about a container such as startup, config, volumes, networking, etc. :

	`docker container inspect`

* Display which port a container is fowarding traffic to:

	`docker container port container_name`

* Attach to a running container:
	
	`docker container attach`

* Build an image from a Dockerfile:

	`docker image build`

* Create a new image from a container's changes:

	`docker container commit`

* Copy files/folders between a container and the local filesystem:

	`docker container cp`

* Create a new container: 

	`docker container create`

* Inspect changes on a container's filesystem:

	`docker container diff`

* Get real time events from the server:

	`docker container system events`

* Run a command in a running container:

	`docker container exec`

* Export a container's filesystem as a tar archive:

	`docker container export`

* Show the history of an image

	`docker image history`

* List images:

	`docker image ls`

* Import the contents from a tarball to create a filesystem image:

	`docker image import`

* Display system-wide information:

	`docker system info`

* Return low-level information on a container, image or task:

	`docker container inspect`

* Kill one or more running container:

	`docker container kill`

* Load an image from a tar archive or STDIN

	`docker image load`

* Log in to a Docker registry:

	`docker login`

* Log out of a Docker registry:

	`docker logout`

* Manage Docker networks:

	`docker network`

* Manage Docker Swarm nodes:

	`docker node`

* Pause all processes within one or more containers:

	`docker container pause`

* List port mapping or a specific mapping for the container

	`docker container port`

* Pull an image or a repository from a registry:

	`docker image pull`

* Push an image or repository to a registry:

	`docker image push`

* Rename a container:

	`docker container rename`

* Restart a container:

	`docker container restart`

* Remove one or more containers:

	`docker container rm`

* Remove one or more images:
	
	`docker image rm`

* Run a command in a new container:

	`docker container run`

* Save one or more images to a tar archive ***(streamed to STDOUT by default)***:

	`docker image save`

* Search Docker Hub for images:

	`docker search`

* Manage Docker services: 

	`docker service`

* Manage Docker Swarm:

	`docker swarm`

* Tag an image into a repository:

	`docker image tag`

* Update configuration of one or more containers:

	`docker container update`

* Display live performance data for all containers:

	`docker container stats`

	##### *** NOTE ***
	The `docker container stats` command does not show the container_name. You can press CTRL + C to cancel stats and then run command `docker container ls -a` to compare performance stats with each unique container_name.


