+++
title = "AWS CLI Configuration"
date = 2021
weight = 2
chapter = false
pre = "<b>4.2 </b>"
+++

In this step, we will generate an IAM user access key and secret access key to use in configuration for the AWS CLI.

1. From [IAM service interface](https://console.aws.amazon.com/iam/home#/home) click **Users**.

![Lightsail](/images/3/00010.png?featherlight=false&width=90pc)

1. Click **Add users*

![Lightsail](/images/3/00011.png?featherlight=false&width=90pc)

2. Name the user **aws-cli**.
  + Click **Programmatic access**, our user only uses it for AWS CLI, so there is no need to log in to the management console.
  + Click **Next: Permissions**.

![Lightsail](/images/3/00012.png?featherlight=false&width=90pc)

3. Click **Attach existing policies directly**.
  + Click on **Administrator Access**.
  + Click **Next: Tags**.

![Lightsail](/images/3/00013.png?featherlight=false&width=90pc)

4. Click **Next: Review**. then click **Create User**.

5. Click **Download .csv** to download the csv file containing access information and secret access key.

![Lightsail](/images/3/00014.png?featherlight=false&width=90pc)

6. Back on our Build Instance run **sudo aws configure** command to proceed with CLI configuration.
  + Configure Region and format information as shown below. Note to use the access key and secret access key from the csv file you downloaded.

![Lightsail](/images/3/00015.png?featherlight=false&width=90pc)

7. The next step is to install Docker to start building the image.

![Lightsail](/images/3/00016.png?featherlight=false&width=90pc)