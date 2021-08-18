> for checking docker version `docker -v`

> starting docker service `service docker start`

> getting docker status `service docker status`

> running docker container `docker run containerName`

> getting all docker running images/containers `docker ps -a`

> list docker images `docker image ls`

> pull the image from registry `docker pull image_name`

> list docker container `docker container ls` or `docker container ls -a`

```javascript
docker run -it ubuntu:latest bash

-i = interactive 
-t = terminal 
ubuntu = imagename 
latest = tag
```

> exit the container it will use inside running bash container `exit`

> for running container `docker run (containerId / containerName)`

> for going inside conatiner `docker attach (containerId / containerName)`

> exit container  without killing container `ctrl + p and q`

> give set of commands for container `docker container --help`

> changeing docker name `docker rename current_name Another_name`

> give stats about container `docker stats container_name`

> give logs of container what happened in container `docker logs container_name > dockerLogFile.txt`

> stop the container `docker stop (containerName / containerID)`

> remove the container `docker rm (containerId / containerName)`

> details about container `docker inspect (containerId / containerName)`

> remove image `docker image rm imageid`

> save one or more image tar archive `docker save -o (imageName.tar) imagename `

> to load tar file which we made tared in another pc/backup `docker load -i (imageName.tar)`

> give new tag `docker tag imagename:tagname imagename:newtagname`

> change the image name `docker tag imagename:tag newname:tag`

> it will remove dangling images which have no name or tag which uses extra space `docker image prune`

> convert docker container into image and save it `docker commit (containerID)`

# Note :-> after upper command give image name and tag

#### Note :-> (create account on hub.docker.com) how to give image name and tag
> `docker tag imageid usenameDockerRegistory/Newname:tag`