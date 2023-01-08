+++
title = "Implement New Deploy"
date = 2021
weight = 6
chapter = false
pre = "<b>4.6 </b>"
+++

In this step, we will deploy the container image to your Lightsail container service.


1. Go to your [Lightsail container service admin interface](https://lightsail.aws.amazon.com/ls/webapp/ap-southeast-1/container-services/lightsail-container/deployments)
  + Click **Deployments**.
  + Click **Modify your deploy**

3. Select **":lightsail-container.nginx-container.hello.x"** container image.
![Lightsail](/images/3/00029.png?featherlight=false&width=90pc)

4. Drag the screen to the bottom and click **Save and Deploy** to deploy.
![Lightsail](/images/3/00030.png?featherlight=false&width=90pc)

5. You will need to wait a few minutes for the deployment to complete.
  + Drag the screen up and wait for the status to change to running.
  + Click on Public domain to access the service running in your container.
![Lightsail](/images/3/00031.png?featherlight=false&width=90pc)

6. The default nginx web page has been replaced with the text **"Welcome to Amazon Lightsail Container workshop"**. Congratulations on completing the Lightsail container lab.

7. After you're done, clean up your resources to avoid unexpected costs.