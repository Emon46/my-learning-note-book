# Docker notes

## build the base image which define in Dockerfile
```
$ docker build .
```
## docker all images show
```
$ docker images
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
## run docker container in localhost 
```
$ docker run -p <localhost_port>:<docker_port> -it <imageID> go run .
```
## stop any docker image 
```
docker stop <imageId>
```
