# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: _______LEVAKU LAKSHMI MOUNIKA_________________________
* **Register Number**: _____212223100026________________
* **Date of Submission**: ______21-05-2026____________

---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

1. First, I logged in to the AWS Management Console and opened the Amazon EC2 dashboard to explore services such as Instances, AMIs, Security Groups, and Key Pairs.

2. Next, I launched a new EC2 instance using the Amazon Linux 2 AMI and selected the `t2.micro` instance type under the free tier. I also created a new key pair and downloaded the `.pem` file.

3. Then, I configured the security group by allowing SSH access on Port 22 from my IP address and HTTP access on Port 80 from anywhere.

4. After the instance was launched, I connected to it using SSH through the terminal with the downloaded key pair and verified that the instance was running successfully.

5. Finally, I performed instance operations such as stop, start, and reboot, monitored the instance metrics in the Monitoring tab, and terminated the instance after completing the experiment to avoid additional AWS charges.


## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List


<img width="1918" height="982" alt="Screenshot 2026-05-21 083624" src="https://github.com/user-attachments/assets/a267574e-9ab4-4bda-8b01-45df336e6861" />


### Screenshot 2: SSH Connection to Instance

<img width="1919" height="964" alt="Screenshot 2026-05-21 090101" src="https://github.com/user-attachments/assets/f6c8caae-f8f6-4d11-be16-b983f1873097" />

<img width="1860" height="967" alt="Screenshot 2026-05-21 083957" src="https://github.com/user-attachments/assets/aaf4c007-792b-4d19-8cb5-abc2e321f907" />

### Screenshot 3: Instance Monitoring / Status

<img width="1918" height="982" alt="Screenshot 2026-05-21 083624" src="https://github.com/user-attachments/assets/1cf0d658-f62b-4cdf-94d5-bfd964cb3b10" />


## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
