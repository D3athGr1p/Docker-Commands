> Step 1 : make file `dockerfile`

> Step 2 : use line `FROM python:2.7` 
##### Note : insted python:2.7 use your prefered image:tag

> Step 3 : `WORKDIR /app`

> Step 4 : `CPY . /app` use your prefred commands to setup container

# Note :-> after upper command give image name and tag

> Step 5 : `CMD ["python", "hello.py"]`

> Step 6 : `docker build .`
##### Note : run this command where dockerfile is

> Step 7 : Now image will be created

> Step 8 : Give the name of this image upload it or share it have a fun.



```javascript
DOCKERFILE DIRECTIVE :
FROM : base image (FROM python:2.7)
COPY : copy file to host to container    (COPY . /app)(copy every things from . to incontariner /app)
WORKDIR : change working directory (WORKDIR /app)
CMD : run command (CMD ["python", "hello.py"])
RUN : run commands and commit the changes in container
ADD : copy amyfiles from host to container (USE COPY INSTED)
ENTRYPOINT : run commands every time container runs
VOLUME : create mount points for externally-mounted volume or other containers
USER : create new users inside container (anycommand run will run using this user)
ARG : define build time variable
ONBUILD : adds a triger instruction when the image is used as the base for another image
STOPSIGNAL : sets the system call signal that will be sent to the container to exit
LABEL : apply key-value metadata to the image, container or daemon.
EXPOSE : expose port outside the world from this container (EXPOSE 80)
```

```javascript
FROM python:2.7
COPY . /app
WORKDIR /app
CMD ["python", "hello.py"]
EXPOSE 80
```