> Step 1 : pull docker image from hub.docker.com
```javascript
sudo docker run -it ubuntu:latest bash
(insted using ubuntu:latest use your prefrence)
```

> Step 2 : do your modifications in docker.

> Step 3 : `exit`

> Step 4 : convert docker container into image and save it `docker commit (containerID)`

# Note :-> after above command give image name and tag

#### Note :-> (create account on hub.docker.com) how to give image name and tag
> Step 5 : `docker tag imageid usenameDockerRegistory/Newname:tag`

> Step 6 : how to upload on (hub.docker.com) `docker login`

> Step 7 : Enter user credentials and the `docker push repoName:tag`

> Step 8 : insted of doing step 6, 7 use `docker save -o (imageName.tar) imagename` and share it.