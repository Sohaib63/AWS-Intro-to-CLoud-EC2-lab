# AWS-Intro-to-CLoud-EC2-lab
# Lab 2: Introduction to Amazon EC2

## Lab overview and objectives

This lab provides you with a basic overview of launching, resizing, managing, and monitoring an Amazon Elastic Compute Cloud (Amazon EC2) instance.

Amazon EC2 is a web service that provides resizable compute capacity in the cloud. It is designed to make web-scale cloud computing simple and intuitive to use.

With the web service interface of Amazon EC2, you can obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources. You can run application servers, blogs, batch processing, and more on the Amazon computing environment. Amazon EC2 reduces the time required to obtain and boot new server instances to minutes so that you can quickly scale capacity both up and down as your computing requirements change.

Amazon EC2 changes the economics of computing so that you pay for only the capacity that you actually use. Amazon EC2 provides developers the tools to build failure-resilient applications and isolate themselves from common failure scenarios.

## Objectives

After completing this lab, you will know how to:

1. Launch a web server with termination protection enabled
2. Monitor Your EC2 instance
3. Modify the security group that your web server is using to allow HTTP access
4. Resize your EC2 instance to scale
5. Explore Amazon EC2 limits
6. Test termination protection
7. Terminate your EC2 instance

## Duration

This lab requires approximately 45 minutes to complete. You will have a total time of 180 minutes to complete this lab.

## AWS service restrictions

In this lab environment, access to AWS services and service actions might be restricted to the ones that are needed to complete the lab instructions. You might encounter errors if you attempt to access other services or perform actions beyond the ones that are described in this lab.

## Accessing the AWS Management Console

At the top of these instructions, choose Start Lab to launch your lab.

A Start Lab panel opens, and it displays the lab status.

Tip: If you need more time to complete the lab, choose the Start Lab button again to restart the timer for the environment.

Wait until you see the message Lab status: ready, then close the Start Lab panel by choosing the X.

At the top of these instructions, choose AWS.

This opens the AWS Management Console in a new browser tab. The system will automatically log you in.

Note: If you find a dialog prompting you to switch to the new console home, choose Switch to the new Console Home.

Tip: If a new browser tab doesn't open, a banner or icon is usually at the top of your browser with a message that your browser is preventing the site from opening pop-up windows. Choose the banner or icon and then choose Allow pop ups.

Arrange the AWS Management Console tab so that it displays along side these instructions. Ideally, you will be able to see both browser tabs at the same time so that you can follow the lab steps more easily.

Tip: If you would like the lab instructions to display across the entire browser window, you can hide the terminal in the browser panel by unchecking the Terminal checkbox in the top right.
## Task 1: Launching your EC2 instance
In this task, you launch an EC2 instance with termination protection. Termination protection prevents you from accidentally terminating an EC2 instance. You also deploy your instance with a user data script in order to deploy a simple web server.

1. In the AWS Management Console on the Services menu, choose EC2.
2. In the left navigation pane, choose EC2 Dashboard to ensure that you are on the dashboard page.
3. Choose Launch instance, and then select Launch instance.

### Step 1: Name your EC2 instance
Using tags, you can categorize your AWS resources in different ways (for example, by purpose, owner, or environment). This categorization is useful when you have many resources of the same type. You can quickly identify a specific resource based on the tags that you have assigned to it. Each tag consists of a key and a value, both of which you define.

When you name your instance, AWS creates a key-value pair. The key for this pair is Name, and the value is the name you enter for your EC2 instance.

1. In the Name and tags section, for Name, enter `Web-Server`
2. Choose the Add additional tags link.
3. From the Resource types dropdown list, ensure that both Instances and Volumes are selected.

## Step 2: Choose an Amazon Machine Image (AMI)
An Amazon Machine Image (AMI) provides the information required to launch an instance, which is a virtual server in the cloud. An AMI includes the following:

- A template for the root volume for the instance (for example, an operating system or an application server with applications)
- Launch permissions that control which AWS accounts can use the AMI to launch instances
- A block device mapping that specifies the volumes to attach to the instance when it is launched

The Quick Start list contains the most commonly used AMIs. You can also create your own AMI or select an AMI from the AWS Marketplace, an online store where you can sell or buy software that runs on AWS.

Locate the **Application and OS Images (Amazon Machine Image)** section. It is just below the Name and tags section.
In the AMI Machine Image (AMI) box, notice that **Amazon Linux 2 AMI** is selected by default. Keep this setting.

## Step 3: Choose an instance type
Amazon EC2 provides a wide selection of instance types that are optimized to fit different use cases. Instance types comprise varying combinations of CPU, memory, storage, and networking capacity and give you the flexibility to choose the appropriate mix of resources for your applications. Each instance type includes one or more instance sizes so that you can scale your resources to the requirements of your target workload.

In this step, you choose a **t2.micro** instance. This instance type has 1 virtual CPU and 1 GiB of memory.
Keep the default instance type, **t2.micro**.

