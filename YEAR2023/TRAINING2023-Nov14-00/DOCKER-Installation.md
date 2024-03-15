https://docs.docker.com/engine/install/
https://docs.docker.com/engine/install/rhel/

[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo yum remove docker \
                  docker-client \
                  docker-client-latest \
                  docker-common \
                  docker-latest \
                  docker-latest-logrotate \
                  docker-logrotate \
                  docker-engine \
                  podman \
                  runc -y

[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo yum install -y yum-utils
[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo systemctl start docker
[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo systemctl enable docker
[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo systemctl status docker

[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo groupadd docker
[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo usermod -aG docker $USER
[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ sudo reboot now
[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ docker run hello-world
[anup@automation-and-continuous-delivery TRAINING2023-Sep05-00]$ docker images