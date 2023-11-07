+++
title = "Installing Docker on Ubuntu for AWS Lightsail"
date = "2021-01-01"
weight = 3
chapter = false
pre = "<b>4.3 </b>"
+++

In this guide, we'll walk through the process of installing Docker on our AWS Lightsail instance. This is an essential step for building and managing container images. For additional details, you can refer to the Docker's official installation [guide for Ubuntu](https://docs.docker.com/engine/install/ubuntu/).

## Installing Docker

The Docker package available in the default Ubuntu repository might not be the latest version. To ensure we install the most up-to-date version, we'll set up Docker's official repository and install from there. This process includes adding a new package source, the GPG key from Docker to verify the integrity of the packages, and then the installation of the Docker package itself.

1. Update Package List

Begin by updating the list of packages:

```
sudo apt update
```

2. nstall Prerequisites
Next, we'll install prerequisite packages that will let apt use repositories over HTTPS:

```
sudo apt install apt-transport-https ca-certificates curl software-properties-common
```

3.  Add Docker’s Official GPG Key
Now, add the official Docker GPG key to your system:

```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```

4. Add the Docker Repository
Add the Docker repository to APT sources:

```
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```

5. Check Docker Versions
Before installing, you can check the versions of Docker available:

```
apt-cache policy docker-ce
```

6. Install Docker
Now we can install Docker:

```
sudo apt install docker-ce
```

7. Verify Docker Service
After the installation, ensure that the Docker service is running:

```
sudo systemctl status docker

```

8. Test Docker Installation
Verify that Docker was installed successfully by running the Hello World image:

```
sudo docker run hello-world
```

![Lightsail](/images/3/00021.png?featherlight=false&width=90pc)

9. Next Steps
With Docker installed, the next step is to build the container image for our application deployment.


![Lightsail](/images/3/00022.png?featherlight=false&width=90pc)