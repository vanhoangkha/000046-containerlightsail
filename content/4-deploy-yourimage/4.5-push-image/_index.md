+++
title = "Push your container image"
date = 2021
weight = 5
chapter = false
pre = "<b>4.5 </b>"
+++

In this step, we will push the container image to the Lightsail store in preparation for deployment to your Lightsail container service.


1. Run the following command to push our container image to the Lightsail store.
```
sudo aws lightsail push-container-image --service-name lightsail-container --label nginx-container-hello --image nginx-container
```
After successful push, Lightsail result will return as below.
```
Image "nginx-container" registered.
Refer to this image as ":lightsail-container.nginx-container.hello.1" in deployments.
```
![Lightsail](/images/3/00025.png?featherlight=false&width=90pc)
{{%notice tip%}}
If you run the command multiple times, push an image multiple times, the number after the image name will increase the sequence number by the number of times you do the push.
{{%/notice%}}

2. Go to the admin interface [Lightsail container](https://lightsail.aws.amazon.com/ls/webapp/ap-southeast-1/container-services/lightsail-container/images)
  + Click the **Images** tab.
  + Here you can see the container images you have pushed.

![Lightsail](/images/3/00026.png?featherlight=false&width=90pc)

3. The next step we will perform a new deployment using the container image you just pushed.