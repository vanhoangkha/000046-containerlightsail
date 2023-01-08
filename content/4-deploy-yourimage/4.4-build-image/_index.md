+++
title = "Build your container image"
date = 2021
weight = 4
chapter = false
pre = "<b>4.4 </b>"
+++

In this step, we will proceed to build the container image to deploy to your Lightsail container service.
Our container image still uses the nginx image but replaces the index.html file to display the greeting.


1. Run the following command to create a directory in preparation for the build image. The next commands will run in this directory.
```
mkdir lightsail-workshop-nginx
cd lightsail-workshop-nginx
```
![Lightsail](/images/3/00021.png?featherlight=false&width=90pc)

2. Run the command below to create the file index.html
```
echo "Welcome to Amazon Lightsail Container workshop" > index.html
```

3. Run the command below to create the Docker file.
```
echo "FROM nginx:latest" > Dockerfile
echo "COPY ./index.html /usr/share/nginx/html/index.html" >> Dockerfile
```
![Lightsail](/images/3/00022.png?featherlight=false&width=90pc)
4. Build our container image by running the following command.
```
sudo docker build -t nginx-container .
```
![Lightsail](/images/3/00023.png?featherlight=false&width=90pc)

5. Run the following command to test the container image we just built on the Build Instance and check the results.
```
sudo docker run -p 8080:80 nginx-container &
curl localhost:8080
```
![Lightsail](/images/3/00024.png?featherlight=false&width=90pc)

6. The next step we will do is push the container image we just created to Lightsail, in preparation for deploying.