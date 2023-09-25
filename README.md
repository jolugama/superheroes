# Docker

Open Desktop docker

## Developer

### Build images
docker-compose build

### Run containers
docker-compose up

### Save docker images in tar
docker images
docker save -o server.tar pruebatecnica-server  
docker save -o angular.tar pruebatecnica-angular 

### Zip client

zip super-hero.zip server.tar angular.tar docker-compose.yml


## Client

### Load images
docker load -i server.tar
docker load -i angular.tar
docker-compose up



