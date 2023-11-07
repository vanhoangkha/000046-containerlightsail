---
title: "Creating a Container Service on AWS"
date: 2021-01-01
weight: 2
chapter: false
pre: "<b>2. </b>"
---

## Creating a Container Service

To get started with Amazon Lightsail's container service, you'll need to follow these steps:

1. Navigate back to the [Lightsail console](https://lightsail.aws.amazon.com/ls/webapp/home/). Select the **Containers** tab.

   ![Lightsail Console - Containers tab](/images/1/0001.png?featherlight=false&width=90pc)

2. Click on the **Create container service** button.

   ![Create container service button](/images/1/0002.png?featherlight=false&width=90pc)

3. Choose a location for your container service by selecting an AWS Region that is either close to you or your customers. For this lab, we'll be using the Singapore Region.

   - Select the container service configuration that meets your needs, which includes memory and processing power. The configuration you choose will determine the compute power, memory, and cost of your container service.

     ![Container Service Configuration](/images/1/0003.png?featherlight=false&width=90pc)

4. Scroll down and name your container service **lightsail-container**, then click on **Create container service**.

   ![Naming and creating container service](/images/1/0004.png?featherlight=false&width=90pc)

5. It will take a few minutes for the container service creation process to complete and for the status to change to Ready. Next, we'll deploy a deployment using a container image from a public repository.

   ![Container Service Creation Process](/images/1/0005.png?featherlight=false&width=90pc)
