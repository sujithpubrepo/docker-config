# docker-config

## Docker Commands
===================
docker search postgres
docker pull postgress:latest
 
docker images

docker run -p 5433:5432 -e POSTGRES_PASWORD=admin postgress
docker run -p 5433:5432 -e POSTGRES_PASWORD=admin --volume postgres_data:/var/lib/docker/volums:/vars/lib/postgressql/data  postgress


docker ps



docker stop some-postgres

## Docker Swarm
==============
docker swarm init
---> docker swarm join --token SWMTKN-1-3cjqixdvfj64x78pmamh4lfrlxc1wb9owyf36z5s6a7ekvazaa-4kxjw4tp8881ef52jrsj9pkb4 192.168.65.4:2377
docker stack deploy --compose-file docker-compose.yml my-swarm

docker stack rm my-swarm
docker events
docker swarm leave --force


## Kubernetes
===========================
