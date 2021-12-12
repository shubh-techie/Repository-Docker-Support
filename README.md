# Repository-Docker-Support
Containers:
Problem statement:
----------------------------------------
Web server - NodeJS/Tomcat/IIS
DB - MongoDB/SQL server 
Messaging - Redis [Database, messaging , caching ]
CM - ansible/puppet
---------------------------------------------
long setup time & multiple servers
	1) System admin 
	2) Install the dependencies
	3) Install the software
	4) Sometimes application works in Dev but doesn't work in QA and production, missing dependencies
=============================
Why we install different apps on different servers
Compatibility issues - all software has dependency and libraries, underlying software.
1) IIS 8.5 
2) Tomcat
-----------------------------------------------
	- To over come the above motioned issues, we can use containers which are isolated environments with their own processes, services, network interface just like a VM, except they share a common OS kernel.
	- Docker is a company which offers free software which helps us to use the container technology.
	- Docker image: Package or a Template of the software or service with its lib & dep.
	- Running instance of image is called container
	


	

              
Install docker
https://docs.docker.com/docker-for-windows/install/

https://docs.docker.com/engine/install/

Registry: it is a repository to keep the images
Azure registry
AWS registry
Docker registry

commands:

docker version - to check version
docker ps - to list running containers 
docker ps -a : to list all containers
docker run  - to pull and run any image from registry (-d option to run as detached or in background)
docker pull - to pull the image on your local machine
docker images: to list the locally downloaded images
docker stop
docker start containerId or name
docker logs containID
docker inspect containerID
docker --name
docker run -p port of host:port of application
docker exec -it containerid bash


docker pull
docker run
i made changes to my webapp
docker commit


Assignment:
Create repository on docker hub and azure container registry
pull a docker image
run it
make changes in docker container
docker commit name
push to docker registry
![image](https://user-images.githubusercontent.com/33177826/145703861-659869e5-d04f-4783-8f6e-3e7a917a7e39.png)
