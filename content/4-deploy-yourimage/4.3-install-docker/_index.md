+++
title = "Install Docker for Ubuntu"
date = 2021
weight = 3
chapter = false
pre = "<b>4.3 </b>"
+++

In this step, we will proceed to install Docker for our Lightsail Instance to build the container image.
You can refer to the installation process [here](https://docs.docker.com/engine/install/ubuntu/)

1. Run the following command to install the necessary packages and add the GPG ( GNU Privacy Guard ) key to be able to use the Docker repository.
```
sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
![Lightsail](/images/3/00018.png?featherlight=false&width=90pc)

2. Run below command to add Docker Repo.
```
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

![Lightsail](/images/3/00019.png?featherlight=false&width=90pc)

3. Install Docker from Repo by running the command below
```
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io -y
```

![Lightsail](/images/3/00020.png?featherlight=false&width=90pc)
 
4. Check the Docker installation with the command below.
```
sudo docker run hello-world
```

![Lightsail](/images/3/00021.png?featherlight=false&width=90pc)

5. The next step we will proceed to build the container image to deploy.


![Lightsail](/images/3/00022.png?featherlight=false&width=90pc)