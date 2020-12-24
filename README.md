# eureka-server

Steps to first deploy

* 01 - sudo apt-get install default-jdk
* 02 - sudo apt install maven
* 03 - sudo apt install git
* 04 - install docker -> https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository
* 05 - sudo mkdir /opt/services



Steps to build and run
* - cd /opt/services
* - sudo git clone https://github.com/eumagnun/eureka-server.git
* - cd eureka-server/eureka-server
* - sudo mvn install
* - sudo docker build -t eumagnun/eureka-server .
* - sudo docker run -d -p 80:8761 eumagnun/eureka-server
