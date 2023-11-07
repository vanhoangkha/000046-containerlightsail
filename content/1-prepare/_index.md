---
title: "Preparation"
date: 2021-01-01
weight: 1
chapter: false
pre: "<b>1. </b>"
---

#### Preparation

Before diving into this lab, ensure you are familiar with the basic concepts necessary to be lab-ready.

**AWS Command Line Interface (CLI)**  
The AWS Command Line Interface (CLI) is a unified tool that enables you to manage AWS services through the command line and scripts. In this lab, you'll be using the AWS CLI to interact with services and deploy an Amazon Lightsail container. Install the AWS CLI by following these instructions:

- [Install AWS CLI](https://aws.amazon.com/cli/)
- [Basic CLI Setup](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)

**AWS Identity and Access Management (IAM)**  
IAM is a service within AWS that helps you securely control access to AWS resources. With IAM, you can manage authentication and authorization for the use of AWS resources.

- [Access Management with IAM](https://aws.amazon.com/iam/)

**Docker**  
Docker provides a platform to develop and run applications within containerized environments. In this lab, you will utilize Docker to build and manage container images, then deploy them on Amazon Lightsail.

#### AWS Lightsail Container Documentation Summary

#### Overview of Container Services
- **Description**: AWS Lightsail containers provide compute resources to deploy Docker images, which are then automatically run on the AWS infrastructure.
- **Source**: [Container services in Amazon Lightsail](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-containers)

#### Creating and Managing Deployments
- **Guide**: Instructions on creating and managing deployments for Lightsail container services.
- **Source**: [Creating and managing deployments for Amazon Lightsail container services](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-creating-and-managing-deployments)

#### Creating Container Services
- **Steps**: Detailed steps for creating a Lightsail container service, including selecting an AWS region through the Lightsail console.
- **Source**: [Creating Amazon Lightsail container services](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-creating-container-services)

#### Container Service Capacity
- **Configuration**: Information on choosing the capacity for a container service, affecting its scale and power.
- **Source**: [Create a Lightsail container service - Amazon Lightsail](https://docs.aws.amazon.com/lightsail/)

#### Managing Container Images
- **Management**: Guidance on pushing and managing container images in Lightsail container services.
- **Source**: [Pushing and managing container images on Amazon Lightsail](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-pushing-and-managing-container-images)

## Creating Container Images
- **Creation**: Steps on creating container images for Lightsail, including running a new container image and building a Dockerfile.
- **Source**: [Creating container images for Amazon Lightsail container services](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-creating-container-images)
