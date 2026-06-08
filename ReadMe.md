# Lab 6 – Scale and Load Balance Your Architecture

## Author

* **Name**: VISHNU RATHAN B
* **Register Number**: 212224240185

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.



## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection



## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch



## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.



## Workflow (To be filled by Student)

1.Review the existing EC2-based application architecture to understand current deployment, resource usage, and scalability requirements before implementing automation.

2.Create a Launch Template that defines EC2 configuration such as AMI, instance type, key pair, security group, and user data. This ensures consistent instance creation in scaling environments.

3.Create an Auto Scaling Group (ASG) using the launch template. Configure minimum, maximum, and desired capacity to automatically manage the number of running instances based on demand.

4.Set up an Application Load Balancer (ALB) and create target groups to distribute incoming traffic evenly across EC2 instances, ensuring high availability and fault tolerance.

5.Attach the ASG to the load balancer, configure scaling policies using CloudWatch alarms (based on CPU utilization), and test by generating traffic to verify automatic scaling and load balancing.

## Output Screenshots 

<img width="1917" height="902" alt="image" src="https://github.com/user-attachments/assets/53bb9459-2bfd-4d21-aea7-ca7d69bbe8cd" />

<img width="1919" height="909" alt="image" src="https://github.com/user-attachments/assets/fd1f41cd-92dd-4f3a-b8cd-36ff33f386b3" />

<img width="1915" height="908" alt="image" src="https://github.com/user-attachments/assets/da7e97a8-f273-407c-8149-cc5cb15e5950" />

<img width="1600" height="856" alt="image" src="https://github.com/user-attachments/assets/a196ed0d-e288-4240-a673-45778f429852" />

<img width="1600" height="937" alt="image" src="https://github.com/user-attachments/assets/14ec1297-7309-493c-af57-2a4c3010614c" />

## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
