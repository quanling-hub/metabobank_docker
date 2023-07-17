## Installation Guide

#### Prerequisites

Before installing the local version of metabobank, you need to install docker and docker-compose first

##### Windows

On Windows need to install WSL first and install the Linux distribution.

We recommend Ubuntu 22.04 LTS

https://apps.microsoft.com/store/detail/ubuntu-22042-lts/9PN20MSR04DW?hl=zh-cn&gl=cn&rtc=1


##### Linux
###### Install docker

**Windows：**

Install and run  Docker Desktop

https://www.docker.com/products/docker-desktop/

**Centos：**

sudo yum install -y yum-utils device-mapper-persistent-data lvm2

sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo

sudo yum install docker-ce

sudo systemctl start docker

sudo systemctl enable docker

**Ubuntu：**

sudo apt-get update 

sudo apt-get install docker.io

###### Install docker-compose

sudo curl -L "https://github.com/docker/compose/releases/download/v2.6.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose

###### Check docker-compose installation

docker-compose version

If you see the following execution result, docker-compose is installed successfully:

`Docker Compose version v2.6.1`

If you encounter problems during the installation process, you can find solutions on docker official site:

- Docker: https://docs.docker.com/engine/install/
  
- Docker Compose: https://docs.docker.com/compose/install/

#### Run Metabobank local version
##### Obtain software release

Git clone metabobank_docker repository

Note: 
     You need to install git and git-lfs in order to clone the repository. You can refer to https://git-scm.com/ and https://github.com/git-lfs/git-lfs/blob/main/INSTALLING.md to install git and git-lfs separately.

##### Run start.sh

Make sure you execute start.sh as root user on bash terminal

./start.sh

##### Visit the metabobank local website

Enter the URL http://local machine ip:8085 or http://127.0.0.1:8085 in your browser

