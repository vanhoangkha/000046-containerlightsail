+++
title = "Clean up resources"
date = 2021
weight = 5
chapter = false
pre = "<b>5. </b>"
+++


We will proceed to delete the resources in the following order

1. Go to [Lightsail container service interface ](https://lightsail.aws.amazon.com/ls/webapp/ap-southeast-1/container-services/lightsail-container/).
  + Click the 3 dots icon.
  ![Lightsail](/images/container/038.png?width=90pc)
  + Click **Delete**
  + Click **Delete container service**.
  ![Lightsail](/images/container/039.png?width=90pc)
  + Click **Yes, delete**.

2. Go to [Lightsail's admin interface](https://lightsail.aws.amazon.com/ls/webapp/home/instances/)
  + Click on the 3-dot icon of the **Build-Instance** instance.
  + Click **Delete**.
  + Click **Yes, delete**.


3. Go to [admin interface of IAM service](https://console.aws.amazon.com/iamv2/home#/users)
  + In the search field, enter **aws-cli**.
  + Click on user **aws-cli**.
  + Click **Delete**.
  ![Lightsail](/images/container/041.png?width=90pc)
  + Enter **aws-cli** to confirm.
  + Click **Delete**.
  ![Lightsail](/images/container/042.png?width=90pc)