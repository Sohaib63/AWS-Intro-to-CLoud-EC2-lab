# AWS-Intro-to-CLoud-EC2-lab
# Introduction to Amazon EC2

In this tutorial, we will be covering the second lab of the "Introduction to Cloud 101" course on AWS Educate, which is the "Introduction to Amazon EC2". The Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides scalable computing capacity in the cloud. This tutorial will guide you through the steps to launch an EC2 instance, connect to it, and perform basic tasks on it.

## Step 1: Log in to the AWS Console

To access the EC2 service, you need to log in to the AWS Console. If you don't have an AWS account, you can create one by visiting the AWS website. 

![Login to AWS Console](images/login.png)

## Step 2: Launching an EC2 Instance

Once you are logged in, navigate to the EC2 dashboard and click on the "Launch Instance" button. In the next screen, select the Amazon Linux 2 AMI. For the instance type, select "t2.micro".

![Launch EC2 Instance](images/launch_instance.png)

## Step 3: Configure the Instance

In the next step, you need to configure the instance. For the purpose of this tutorial, you can use the default settings. However, if you need to, you can configure the instance to your specifications.

![Configure Instance](images/configure_instance.png)

## Step 4: Add Storage

You will also need to add storage to your instance. The default setting is 8 GB, which should be sufficient for this tutorial. If you need more storage, you can increase it.

![Add Storage](images/add_storage.png)

## Step 5: Configure Security Group

A security group acts as a virtual firewall for your instance to control inbound and outbound traffic. In the next step, you need to create a new security group. Add a rule to allow SSH traffic on port 22.

![Configure Security Group](images/configure_security_group.png)

## Step 6: Launch the Instance

Once you have completed the previous steps, you are ready to launch your instance. Click on the "Launch" button, and then select an existing key pair or create a new one. This key pair will be used to log in to the instance.

![Launch Instance](images/launch.png)

## Step 7: Connect to the Instance

Now that your instance is running, you need to connect to it. You can do this using a terminal or a program such as PuTTY. You will need the public IP address of your instance, which you can find in the EC2 dashboard.

![Connect to Instance](images/connect_to_instance.png)

## Step 8: Perform Basic Tasks

Once you have connected to your instance, you can perform basic tasks such as updating packages, installing new software, and creating files. You can also use the EC2 instance to host a website, run a database, or perform other tasks.

![Perform Basic Tasks](images/basic_tasks.png)

## Conclusion

This concludes the tutorial for the "Introduction to Amazon EC2" lab in the "Introduction to Cloud 101" course on AWS Educate. By following the steps outlined in this tutorial, you should now have a basic understanding of how to launch and manage an EC
