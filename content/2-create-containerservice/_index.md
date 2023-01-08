+++
title = "Create container service"
date = 2021
weight = 2
chapter = false
pre = "<b>2. </b>"
+++

#### Create container service

1. Return to the [Lightsail console] interface (https://lightsail.aws.amazon.com/ls/webapp/home/). Click on the **Container** tab.

![Lightsail](/images/1/0001.png?featherlight=false&width=90pc)

Click **Create container service**

2. ![Lightsail](/images/1/0002.png?featherlight=false&width=90pc)

3. Select a location for your container service by selecting an AWS Region near you or near your customer. For this lab, we will use Region Singapore.
  + Choose the level of container service configuration you will need (including memory and processing power). The configuration you choose determines the compute power, memory, and cost of your container service.

![Lightsail](/images/1/0003.png?featherlight=false&width=90pc)

4. Scroll down, name your container service **lightsail-container** then click **Create container service**.

![Lightsail](/images/1/0004.png?featherlight=false&width=90pc)

5. It will take a few minutes for the container service creation to complete and the status to change to Ready. The next step we will perform a deployment from a container image taken from the public repo (public repository).

![Lightsail](/images/1/0005.png?featherlight=false&width=90pc)