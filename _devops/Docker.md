---
title: Docker
permalink: /devops/Docker/
toc: true
published: true
---



### Docker Installtion
- Installation Steps
	- sudo apt update 
    - sudo apt upgrade
    - sudo apt install docker.io -y 
    - systemctl start docker
    - systemctl enable docker
    - docker version

#### Additional Tools

##### [Portainer](https://www.portainer.io/) 
- open-source management UI for Docker
- allows to manage Docker containers, images, networks and volumes
- Installation
	- Installing on **Debian**
	- Requirements 
		- sudo or root permissions
    	- Docker
	 - Installation commands
     			- docker pull portainer/portainer
        		- docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer
       		 	- docker ps
             	- go to http://localhost:9000 and create admin password
        		- choose environment to connect 
        		- if you have docker configuration in local machine, select 'Local' environment


#### Packer https://www.packer.io/intro/getting-started/install.html
##### Vagrant  https://www.vagrantup.com/docs/installation/
