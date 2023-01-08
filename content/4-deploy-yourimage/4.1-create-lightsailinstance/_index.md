+++
title = "Create Lightsail instance"
date = 2021
weight = 1
chapter = false
pre = "<b>4.1 </b>"
+++

In this step, we will create the Lightsail Instance.

1. From the [Lightsail admin interface](https://lightsail.aws.amazon.com/ls/webapp/home/) click **Create Instance**.
![Lightsail](/images/3/0001.png?featherlight=false&width=90pc)
2. Click the **Linux/Unix** platform. Under Blueprint, click **OS Only*, then select **Ubuntu Linux 20.04 LTS**.

![Lightsail](/images/3/0002.png?featherlight=false&width=90pc)

3. Scroll down, under **Identify your instance**, name our instance **Build-Instance**.

![Lightsail](/images/3/0003.png?featherlight=false&width=90pc)

4. Drag the screen down, click **Create Instance**.

![Lightsail](/images/3/0003.png?featherlight=false&width=90pc)

5. Wait a few minutes for the Lightsail instance to switch to the running state as shown below.
 + Click on the command line icon to connect to Build-Instance.

![Lightsail](/images/3/0004.png?featherlight=false&width=90pc)

6. Install the unzip tool for Ubuntu
```
sudo apt-get install -y unzip
```

![Lightsail](/images/3/0005.png?featherlight=false&width=90pc)

7. Install AWS CLI on Build-Instance by running the commands below
```
sudo curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
sudo unzip awscliv2.zip
sudo ./aws/install
```
![Lightsail](/images/3/0006.png?featherlight=false&width=90pc)

8. Install the Lightsail control plugin for AWS CLI by running the commands below
```
sudo curl "https://s3.us-west-2.amazonaws.com/lightsailctl/latest/linux-amd64/lightsailctl" -o "/usr/local/bin/lightsailctl"
sudo chmod +x /usr/local/bin/lightsailctl
```
![Lightsail](/images/3/0007.png?featherlight=false&width=90pc)

9. Next step we will create **awsstudent** user with **Administrator Access** permission, then create accesskey / secret accesskey to configure AWS CLI.

![Lightsail](/images/3/0008.png?featherlight=false&width=90pc)

![Lightsail](/images/3/0009.png?featherlight=false&width=90pc)