### Dockerfile
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker build -t cli-interactive-react-2024:V20 .
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker rmi cli-interactive-react-2024:V20
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker images

[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker build -t cli-interactive-react-2024-image:V20 .

### Docke Image
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker images

### Docker Container
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker run cli-interactive-react-2024-image:V20
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker run -p 3000:3000 cli-interactive-react-2024-image:V20
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker run --rm -d -p 3000:3000 cli-interactive-react-2024-image:V20
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker run --rm -d -p 3000:3000 --name cli-interactive-react-2024-container-3000 cli-interactive-react-2024-image:V20
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker run --rm -d -p 3001:3000 --name cli-interactive-react-2024-container-3001 cli-interactive-react-2024-image:V20
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker ps
[anup@automation-and-continuous-delivery cli-interactive-react-2024]$ docker stop ac29581e61d6

