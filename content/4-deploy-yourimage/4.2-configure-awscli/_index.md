---
title: "AWS CLI Configuration Guide"
date: 2021-01-01
weight: 2
chapter: false
pre: "<b>4.2 </b>"
---

#### Initial Configuration of AWS CLI

Amazon Web Services (AWS) is a versatile and powerful cloud services platform. To manage AWS services efficiently via the Command Line Interface (CLI), you need to set up the AWS CLI by creating access keys for an IAM User. Here is a step-by-step guide to facilitate this process for you.

**Step 1:** Log in to the AWS Management Console
- Access the AWS Management Console at the following link: [https://console.aws.amazon.com/iam/](https://console.aws.amazon.com/iam/).

**Step 2:** Select an IAM User
- In the IAM console, go to "Users" in the navigation pane and click on the username for whom you want to create an access key.

**Step 3:** Create an Access Key
- On the user's details page, navigate to the "Security credentials" tab and, within the "Access keys" section, click "Create access key".

**Step 4:** Configure the Access Key in the CLI
- During the configuration process, select "Command Line Interface (CLI)".

**Step 5:** Enter Tags (if necessary)
- You may enter tags for the access key if desired, then click "Next".

**Step 6:** Download the .csv File
- Click on "Download .csv file" to download a file containing the access key ID and secret access key.

**Step 7:** Complete Key Creation
- After the .csv file has been downloaded, click "Done" to finish.

**Important Note:** An access key is sensitive data and should be kept secure. Store the .csv file carefully and do not share it with untrusted individuals.

Following these steps makes creating and configuring the AWS CLI simple, enabling flexible management of AWS resources via the CLI.
