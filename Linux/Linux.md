# Linux
Common commands and how-to's for Linux

## Table of Contents
* [Common Commands](#common-commands)
* [Docker Commands](#docker-commands)

### Common Commands
* cp : Copy file or directory
* cp -r : Copy folder recursively
* mv : Move file or folder
* mv -r : Move folder recursively
* rm : remove file or folder
* rm -f : Force delete file or folder
* mkdir : Make directory

### Docker Commands
* service docker start/stop : To start/stop docker service
* docker ps : Show the running containers
* docker ps -a : Show all the containers
* docker images : Show all the container images
* docker rm : Remove container (-f to force delete)
* docker rmi : Remove image
* docker build -t name:version path/to/dockerfile : To build a docker image with 'name' and 'version'
``` bash
docker build -t tomcat:8 .
```
* docker run -d IMAGE -p 8080:8080 --name dockerName : To run a docker image on a container 
``` bash
docker run -d tomcat -p 80:8080 -p 443:8443 --name secureassist
```

### Unzip and Tar Commands
* tar -xvzf : Unzip the tar file into a folder
* unzip : Unzip the zip file
* unzip filename.zip -d path/to/folder : Unzip to mentioned folder
