# Docker

Open Desktop docker

## Developer

### Build images
docker-compose build

### Run containers
docker-compose down
docker-compose up --build

### Save docker images in tar
docker images
docker save -o server.tar pruebatecnica-server  
docker save -o angular.tar pruebatecnica-angular 

### Zip client

zip super-hero.zip server.tar angular.tar docker-compose.yml


## Client

### Load images and run
docker load -i server.tar
docker load -i angular.tar
docker-compose up

docker run -d -p 3000:3000 --name my-server pruebatecnica-server
docker run -d -p 4200:4200 --name my-angular-app pruebatecnica-angular



