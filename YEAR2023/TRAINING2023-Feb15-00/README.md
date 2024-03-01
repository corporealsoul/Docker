# Docker

▐░░░░░░░░░░░░░▌▐░░░░░░░░░░░░░▌▐░░░░░░░░░░░░░▌ TRAINING2023-Feb15-00- Spiral Pad : DOCKER RUNTIME

PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker version
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker --version

PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker images
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker pull nginx
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker pull nginx:1.25

PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker scout quickview nginx:1.25

PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker run nginx:latest
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker run -d nginx:latest
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker logs 3453a4ac7c94cb478124a22454243e594d221ba50975bbd79b671634244a87ed
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker stop 3453a4ac7c94cb478124a22454243e594d221ba50975bbd79b671634244a87ed

PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker run -d -p 8000:80 nginx
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker stop c9393fac95c7

PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker run --name web-app -d -p 8000:80 nginx

PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker rm $(docker ps -a -q)
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker rm $(docker ps --all --quiet)
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker rmi $(docker images -q)

PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker container prune
PS D:\GITRepos\Docker\YEAR2023\TRAINING2023-Feb15-00> docker image prune