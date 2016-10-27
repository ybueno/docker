# docker

udo apt-get update
sudo apt-get install apt-transport-https ca-certificates
sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D
deb https://apt.dockerproject.org/repo ubuntu-trusty main

sudo apt-get purge lxc-docker 

apt-cache policy docker-engine 

sudo apt-get install linux-image-extra-$(uname -r) linux-image-extra-virtual 

sudo apt-get install docker-engine
sudo service docker start

# criar container
docker images
docker build -t nginx-example . (pasta local)

# rodar e exibir o terminal (/bin/bash)
#porta docker:porta maquina
docker run -p 80:80 -it 57a669e19303 /bin/bash

CTRL + D para sair


# para remover
docker images
docker rmi -f ID

#exibir containers
docker ps -a


