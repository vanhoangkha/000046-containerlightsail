+++
title = "Deploy public image"
date = 2021
weight = 3
chapter = false
pre = "<b>3. </b>"
+++


#### Deploy container from public image


1. Click **Deployments** tab.
  + Click **Create your first deployment**.

![Lightsail](/images/2/0001.png?featherlight=false&width=90pc)

2. Set the caontainer name and image name **nginx**.
Soure container images can come from a public repository, like Docker Hub, or are container images that you've created and hosted using your container image repo service.
For this lab, we will use the official Nginx docker container image provided by Nginx. Docker Official Images is a curated collection of Docker repositories hosted on Docker Hub that have been scanned for vulnerabilities and are maintained by the Docker team.

![Lightsail](/images/2/0002.png?featherlight=false&width=90pc)

3. You can also add optional configurations such as initial launch commands, environment variables and network ports for the container.
For this lab, you don't need to specify the launch command or environment variables, but you need to open the port to connect to the nginx server.
We will configure the Nginx Container to listen on port 80 for HTTP traffic.
  + Click **Add open ports**.

![Lightsail](/images/2/0003.png?featherlight=false&width=90pc)

4. Fill in port information **80**. Protocol remains **HTTP**.

![Lightsail](/images/2/0004.png?featherlight=false&width=90pc)

5. To test the container service is working correctly, we will need to define a public endpoint that we can navigate to in our web browser.
We will specify nginx as the container and handle the traffic to the public endpoint via port 80. The health check (/) path will be left at the default value.
  + Click **Save and deploy**.

![Lightsail](/images/2/0005.png?featherlight=false&width=90pc)


6. It will take a few minutes for the container deployment to complete and the status to change from **Deploying** to **Active**.

![Lightsail](/images/2/0006.png?featherlight=false&width=90pc)

7. Drag the screen upwards and click on the **public domain** of the deployment to connect to the nginx container.

![Lightsail](/images/2/0007.png?featherlight=false&width=90pc)

8. You will connect to the nginx server installed in your nginx container. You have deployed the container using the public container image from Docker Hub. The next step, we will manually create the container image and deploy it on the Lightsail container service.

![Lightsail](/images/2/0008.png?featherlight=false&width=90pc)