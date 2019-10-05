# traefik-v1-example
An example of traefik + docker

### To use this example you must have docker and docker-compose installed on your machine. ###

# Instructions

### 1- Download repository
   git clone https://github.com/marcelloti/traefik-v1-example
   
### 2- Create docker networks
   docker network create web && docker network create internal

### 3- Put DNS records on hosts (on linux usually in /etc/hosts):
127.0.0.1 www.monitor.local

127.0.0.1 www.whoami.local

### 4- Run docker-compose
cd traefik-v1-example

docker-compose -p example up -d

### 5- Access the traefik Dashboard
http://www.monitor.local/dashboard 

User: admin / Password: admin
