# Linux
Common commands and how-to's for Linux

## Table of Contents
* [Common Commands](#common-commands)
* [Docker Commands](#docker-commands)
* [Unzip and Tar Commands](#unzip-and-tar-commands)
* [Start and Stop Service](#start-and-stop-service)
* [User Management]()


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
* docker run -d IMAGE -p 8080:8080 --name containerName : To run a docker image on a container 
``` bash
docker run -d tomcat -p 80:8080 -p 443:8443 --name secureassist
```
* docker exec -it containerName bash : Opens a bash terminal in the container
* docker cp containerName:path/to/copy/from/ path/to/copy/to
* docker cp path/to/copy/from containerName:path/to/copy/to


### Unzip and Tar Commands
* tar -xvzf : Unzip the tar file into a folder
* unzip : Unzip the zip file
* unzip filename.zip -d path/to/folder : Unzip to mentioned folder


### Start and Stop Service
* service tomcat start : Start tomcat service
* service tomcat stop : Stop tomcat service
* systemctl start/restart/stop tomcat : Another way to start/restart and stop tomcat 

### User Management
* adduser <username> : Create a new user, replace <username>
* passwd : Change the password of current user
* passwd <username> : Change password of this user, replace <username>
* userdel -r <username> : Delete the user and his home dir
