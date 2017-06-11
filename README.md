# DOCKER CHEATSHEET
This is a list of commonly used [Docker](https://www.docker.com/) commands for any "Dockerized" app development workflow for developers.

### What's Docker and why use it?
Docker is the world's leading software container platform. Developers use Docker to eliminate the "works on my machine" problems when collaborating on code. Regardless if your OS is Mac, Windows, or a Linux Distro, Docker apps are completely portable and platform agnostic. Docker also manages and tracks changes and dependencies, which makes it easier for sysadmins to understand how the apps works.

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

* Display all images: 
`docker images`

* List your running containers **(old command: docker ps)**
`docker container ls`
`docker container ls -a (-a flag lists all containers running or not)`


