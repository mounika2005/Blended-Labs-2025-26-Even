# Build Your VPC and Launch a Web Server (AWS) 

## Author

* **Name**: ___Levaku Lakshmi Mounika_____________________________
* **Register Number**: _______212223100026______________
* **Date of Submission**: _____16/052026_____________

---

## Objective

The objective of this experiment is to understand how to design and configure a basic network infrastructure in AWS using a Virtual Private Cloud (VPC). This lab focuses on creating a VPC with a public subnet, configuring an Internet Gateway and route table, launching an EC2 instance, and hosting a simple web server that can be accessed over the internet.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity

---

## Tools Used

* AWS Management Console
* Amazon VPC
* Amazon EC2
* Internet Gateway
* Route Table
* Security Groups

---

## Tasks Performed

### Task 1: Create a VPC

Create a new Virtual Private Cloud (VPC) with a private IP address range. The VPC acts as a logically isolated network in AWS where all other resources will be deployed.

Students should create a VPC with an appropriate CIDR block (for example, 10.0.0.0/16) and assign a meaningful name.


### Task 2: Create a Public Subnet

Create a subnet inside the VPC to host public resources. Enable auto-assign public IPv4 so that instances launched in this subnet receive a public IP address.

The subnet should use a smaller CIDR range (for example, 10.0.1.0/24).


### Task 3: Create and Attach Internet Gateway

Create an Internet Gateway (IGW) and attach it to the VPC. This allows communication between resources in the VPC and the internet.


### Task 4: Configure Route Table

Create a route table and add a default route (0.0.0.0/0) pointing to the Internet Gateway. Associate this route table with the public subnet.

This step ensures that traffic from the subnet can reach the internet.


### Task 5: Create Security Group

Create a security group to act as a virtual firewall for the EC2 instance. Configure inbound rules to allow:

SSH on port 22

HTTP on port 80


### Task 6: Launch EC2 Instance

Launch an EC2 instance inside the public subnet using Amazon Linux 2 AMI and a suitable instance type (t2.micro).

Attach the previously created security group and key pair.


### Task 7: Configure Web Server

Install and start a web server (Apache HTTPD) on the EC2 instance using user data or manual commands.

Create a simple HTML page and verify that it can be accessed from a web browser using the public IP address of the instance.---

## Workflow (Student Explanation)

1. Logged into the AWS Management Console and opened the VPC Dashboard. Created a new VPC with CIDR block 10.0.0.0/16 and assigned a name to the VPC.

2. Created a public subnet inside the VPC with CIDR block 10.0.1.0/24 and enabled auto-assign public IPv4 address option.

3. Created an Internet Gateway and attached it to the VPC. Then created a Route Table, added a default route (0.0.0.0/0) to the Internet Gateway, and associated the route table with the public subnet.

4. Created a Security Group and configured inbound rules to allow SSH traffic on port 22 and HTTP traffic on port 80.

5. Launched an EC2 instance using Amazon Linux 2 AMI and t2.micro instance type. Attached the created security group and key pair to the instance.

6. Connected to the EC2 instance and installed the Apache HTTP web server using Linux commands.

7. Created a simple HTML webpage, started the Apache service, and verified the web server by accessing the EC2 public IP address in a web browser.

---

## Output Screenshots (Attach 3)

### Screenshot 1: VPC and Subnet Details

<img width="1911" height="912" alt="Screenshot 2026-05-17 222726" src="https://github.com/user-attachments/assets/1752d1b2-a6d2-4525-a59a-847d6d02e5d8" />


---

### Screenshot 2: EC2 Instance Running


<img width="1904" height="967" alt="Screenshot 2026-05-17 225059" src="https://github.com/user-attachments/assets/53804cb6-7322-4d0e-88a2-466ad488850a" />

---

### Screenshot 3: Web Server Output in Browser
<img width="1913" height="1031" alt="Screenshot 2026-05-17 225506" src="https://github.com/user-attachments/assets/4da8a534-d73b-4843-ae85-6656ea964df8" />


---

## Result 

This experiment successfully demonstrated the creation of a custom VPC and deployment of a public-facing web server in AWS. By configuring networking components such as subnets, route tables, and security groups, and by launching an EC2 instance with a web server, the basic architecture of a cloud-hosted application was understood.
