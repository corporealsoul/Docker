<br>

▐░░░░░░░░░░░░░▌▐░░░░░░░░░░░░░▌▐░░░░░░░░░░░░░▌


**https://docs.docker.com/engine/install/**

**https://docs.docker.com/engine/install/rhel/**

<br>

### Uninstall old versions

    [anup@infrastructure-management-and-provisioning ~]$ sudo yum remove docker \
                      docker-client \
                      docker-client-latest \
                      docker-common \
                      docker-latest \
                      docker-latest-logrotate \
                      docker-logrotate \
                      docker-engine \
                      podman \
                      runc

<br>

### Set up the repository

`[anup@infrastructure-management-and-provisioning ~]$ sudo yum install -y yum-utils`

`[anup@infrastructure-management-and-provisioning ~]$ sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo`

<br>

### Install Docker Engine

`[anup@infrastructure-management-and-provisioning ~]$ sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin`

`[anup@infrastructure-management-and-provisioning ~]$ docker version`

`[anup@infrastructure-management-and-provisioning ~]$ docker --version`

<br>

### Start and Enable Docker

`[anup@infrastructure-management-and-provisioning ~]$ sudo systemctl start docker`

`[anup@infrastructure-management-and-provisioning ~]$ sudo systemctl enable docker`

`[anup@infrastructure-management-and-provisioning ~]$ sudo systemctl status docker`

<br>

### Verify that the Docker Engine installation is successful by running the hello-world image.

`[anup@infrastructure-management-and-provisioning ~]$ sudo docker run hello-world`

<br>

### Linux post-installation steps for Docker Engine

`[anup@infrastructure-management-and-provisioning ~]$ sudo groupadd docker`

`[anup@infrastructure-management-and-provisioning ~]$ sudo usermod -aG docker $USER`

`[anup@infrastructure-management-and-provisioning ~]$ newgrp docker`

`[anup@infrastructure-management-and-provisioning ~]$ docker run hello-world`

<br>

