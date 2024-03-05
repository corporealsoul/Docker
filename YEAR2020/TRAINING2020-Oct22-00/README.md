# Docker

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker ps
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker images

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker pull redis
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker images

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker run redis 

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker ps -a
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker start 0a4d726c3fee
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker stop 0a4d726c3fee

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker run -d redis:7.2

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker run -d -p 6000:6379 redis
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker run -d -p 6001:6379 redis:7.2
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker ps

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker logs 8f77385ad0f6

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker run -d -p 6000:6379 --name my-redis redis
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker ps

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker exec -it 0a516895de04 /bin/bash
root@0a516895de04:/data# cat /etc/os-release 

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker network ls
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker network create mongo-network
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker pull mongo  
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker scout quickview mongo
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker pull mongo-express



PROJECT :
https://hub.docker.com/_/mongo
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker run -d -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=password --name mongo --net mongo-network mongo
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker ps
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker logs ad7c75e5795f

https://hub.docker.com/_/mongo-express
PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker run -d -p 8081:8081 -e ME_CONFIG_MONGODB_ADMINUSERNAME=admin -e ME_CONFIG_MONGODB_ADMINPASSWORD=password -e ME_CONFIG_MONGODB_SERVER=mongo --name mongo-express --network mongo-network mongo-express

http://localhost:8081/

PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker ps


DOCKER COMPOSE,


DOCKERFILE,


DOCKER REGISTRY



