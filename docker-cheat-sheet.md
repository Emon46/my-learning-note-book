# Docker notes

## build the base image which define in Dockerfile
```
$ docker build .
```
## docker all images show
```
$ docker images
```
## delete a image
```
$ docker image rm [image name]
```
## delete all existing image
```
$ docker image rm $(docker images -a -q)
```
## Delete a specific container (only if stopped).
```
$ docker rm [container name]
```
## Delete all containers (only if stopped).
```
$ docker rm $(docker ps -a -q)

```
## Display logs of a container.
```
$ docker logs [container name]
```
## all running docker container 
```
$ docker ps
```
## all container exited and running
```
$ docker ps -a
```
## Build a docker image 
```
$ docker build . -t <repository_name>:<tag_name>
```
## alias (a reference) by the name of the TARGET_IMAGE
```
$ docker tag SOURCE_IMAGE[:TAG] TARGET_IMAGE[:TAG]
```
## run docker container in localhost 
```
$ docker run -p <localhost_port>:<docker_port> -it <imageID> go run .
```
```
$  docker container run --publish 8000:8080 --detach --name <the_name_you_want_to_mention> <repository_name>:<tag_name>
```
<b>-p or --publish :</b> asks Docker to forward traffic incoming on the localhost’s port , to the container’s port . Containers have their own private set of ports, so if you want to reach one from the network, you have to forward traffic to it in this way. Otherwise, firewall rules will prevent all network traffic from reaching your container, as a default security posture.</br>
<b>--detach :</b> asks Docker to run this container in the background.</br>
<b>--name :</b> specifies a name with which you can refer to your container in subsequent commands, in this case bb.

## The --force option removes the running container.
```
docker container rm --force <name_that_given_by_you>
```
## stop any docker container 
```
$ docker stop <imageId>
```
## stop all docker container 
```
$ docker stop $(docker ps -a -q)
```
## Use the official image as a parent image
```docker
FROM node:current-slim
```

# Set the working directory
```docker
WORKDIR /usr/src/app
```
# Copy the file from your host to your current location
```docker
COPY package.json .
```
# Run the command inside your image filesystem
```docker
RUN npm install
```
# Inform Docker that the container is listening on the specified port at runtime.
```docker
EXPOSE 8080
```
# Run the specified command within the container.
```docker
CMD [ "npm", "start" ]
```
# Copy the rest of your app's source code from your host to your image filesystem.
```docker
COPY . .
```
