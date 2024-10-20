<h1 align="center"> Docker </h1>

<dl>
  
  <h2> Docker Information </h2>

```bash
# This command with give the version of the docker installed in the system
docker -v

# This command will give the information about the docker
docker info
```

<h2> Docker Image List </h2>

```bash
# This command will list all the docker images
docker images
```

<h2> Docker Container List </h2>

```bash
# This command lists all the running containers
docker ps

# This command list all the containers
docker ps -a
```

<h2> Docker Search For Images </h2>

```bash
# This command search for the images in the docker hub.
#Example docker search mysql
docker search <image-name>

```

<h2> Pull Docker Images </h2>

```bash
#This command pulls the docker images from the dockerhub
docker pull <image-name>:<tag> #here tag is optional and if no tags are provided then it takes the latest tag automatically
```

<h2> Running Docker Images </h2>

```bash
#This command runs the docker image
#example docker run python:latest
docker run <image-name>:<tag> #if the tag is latest then it is optional , this is a mini

# This command will run the container in the background and return with the container id
docker run -d <image-name>:<tag>

# this command will run the container in the interactive way and provide with the terminal
docker run -it <image-name>:<tag>

# Adding --name flag helps us to give the custom name of the container and this flag is optional but better to use in practice
#Example docker run --name python -it -d python:latest
docker run --name <custom-name> <image-name>:<tag>
```

<h2> Inspect about a particular container </h2>

```bash
# This command will inspect the particular container
docker inspect <container-id>
```

<h2> Getting logs about the container </h2>

```bash
# This command will Log the information in the container such as error message
docker log <container-name>
```

<h2> Execute command for the container running in the background </h2>

```bash
# This command will execute the command in the container running in the background
# Example: docker exec -it python python3
docker exec <flags> <container-name> <command> # container name can be replaced with the container id
```

<h2> Start, Stop and Restart the existing container </h2>

```bash
# This command will start the container
docker start <container-name>

# This command will stop the container
docker stop <container-name>

# This command will restart the container
docker restart <container-name>

# Container name are replaceable with the container id

```

<h2> Remove the container and images </h2>

```bash
# This command will remove the container with the particular name
docker rm <container-name>

# This command will delete all the container at once
docker container prune

# To Remove the docker images we need to make sure that all the containers having that images are removed

# This command will delete the particular docker image
docker rmi <image-name>

# This command will delete all the docker images at once
docker system prune
```

<h2> Docker Issue in Ubuntu 22.04 latest version </h2>
<h3> In ubuntu, there might be a issue that the docker desktop may not open. This is because ubuntu has restricted some privileges. To fix the issue we can run </h3>

```bash
# This command will change the restricted privileges
sudo sysctl -w kernel.apparmor_restrict_unprivileged_userns=0

# This command will run the docker desktop (can use the gui also)
systemctl --user start docker-desktop
```

</dl>
