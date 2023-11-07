---
title: "Deploying a Public Image"
date: 2021
weight: 3
chapter: false
pre: "<b>3. </b>"
---

## Deploying a Container from a Public Image

1. Navigate to the **Deployments** tab.
   - Click on **Create your first deployment**.

   ![Lightsail](/images/2/0001.png?featherlight=false&width=90pc)

2. Name your container (`container name`) and set the image name (`image name`) to **nginx**.
   The source container image can originate from a public repository like Docker Hub or your own container images stored on a personal container image repo service.
   In this lab, we'll employ the official Nginx docker image, provided by Nginx. Docker Official Images are a curated set of Docker repositories hosted on Docker Hub, security-scanned for vulnerabilities, and maintained by the Docker team.

   ![Lightsail](/images/2/0002.png?featherlight=false&width=90pc)

3. You may also add optional configurations such as initial run commands, environment variables, and network ports for your container.
   For this lab, there's no need to specify any initial commands or environment variables, but you will need to open a port to connect to the nginx server.
   We'll configure the Nginx Container to listen on port 80 for HTTP traffic.
   - Click on **Add open ports**.

   ![Lightsail](/images/2/0003.png?featherlight=false&width=90pc)

4. Enter the information for the port as **80** and leave the Protocol as **HTTP**.

   ![Lightsail](/images/2/0004.png?featherlight=false&width=90pc)

5. To verify that the container service is functioning correctly, we need to determine the public endpoint that can be accessed via a web browser.
   We will designate nginx to handle traffic to the public endpoint over port 80. The health check path (`/`) will retain its default value.
   - Click on **Save and deploy**.

   ![Lightsail](/images/2/0005.png?featherlight=false&width=90pc)

6. The container deployment process may take a few minutes to complete, with the status transitioning from **Deploying** to **Active**.

   ![Lightsail](/images/2/0006.png?featherlight=false&width=90pc)

7. Scroll up and click on the deployment's **public domain** to connect to the nginx container.

   ![Lightsail](/images/2/0007.png?featherlight=false&width=90pc)

8. You are now connected to the nginx server installed on your nginx container. This container has been deployed using a public container image from Docker Hub. Next, we'll proceed to create our own container image and deploy it on the Lightsail container service.

   ![Lightsail](/images/2/0008.png?featherlight=false&width=90pc)
