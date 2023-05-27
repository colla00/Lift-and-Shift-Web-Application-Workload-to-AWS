# Lift and Shift Web Application Workload to the Cloud. Amazon Web Service (AWS)
## DevOps Project-3
#### Project Source: [DevOps Project](https://www.udemy.com/course/devopsprojects/learn/lecture/23885400#overview) by Alexis Collier

In this Project, We will be using the LIFT AND SHIFT strategy  for our web application setup. 
Lift And Shift is a strategy involves the migration of an application or a code base from a local setup(such as  data center or VMs) to a cloud environment,in this case AWS . I will be migrating a java based  application that was setup in my previous. Link to the project 1
This Project Aims to solve cost and scalability challenges building running your application locally (Data center). 

# AWS SERVICES USED

- Elastic Compute Cloud (EC2) 
- Elastic Load Balancer (ELB)
- Auto-scaling
- S3 bucket
- Amazon Certificate Manager (ACM)
- Route 53
- Security Group
- EFS

### Other Tools Used are
- DNS resolution
- jdk8
- maven

# Project Architecture on AWS

![](https://github.com/Adutoby/DevOps-Projects-AWS/blob/master/Project-3:%20Lift%20And%20Shift%20Web%20Application%20to%20AWS/images/project%20architecturenew.png)

picture credit: rumeysakdogan

# Flow of Execution
1. Log into your AWS account
2. Create security groups for the backend services
3. Create Key pairs to login into server
4. Lunch EC2 instance with user data (BASH SCRIPTS)
5. Update IP to name mapping in route 53
6. Build Our Application from source code
7. Upload our Application to S3 bucket
8. Download artifact to Tomcat EC2 Instance
9. Setup ELB with HTTPS [certificate from (ACM)Amazon certificate manager
10. Map ELB Endpoint to website name in Amazon route 53 and Verify
11. Configure Auto Scaling Group for the Application Instance and Verify
