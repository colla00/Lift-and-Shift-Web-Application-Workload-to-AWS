# Lift and Shift Web Application Workload to Amazon Web Services
## DevOps Project-3
#### Project Source: [DevOps Project](https://www.udemy.com/course/devopsprojects/learn/lecture/23885400#overview) by Imran Teli

The Lift And Shift strategy involves migrating an application or a code base from a local setup (such as a data center or VMs) to a cloud environment, in this case, AWS. This project aims to solve cost and scalability challenges by building and running the application locally (data center). 

# AWS Services Used:

- Elastic Compute Cloud (EC2)  
- Elastic Load Balancer (ELB)
- Auto-scaling
- S3 Bucket
- Amazon Certificate Manager (ACM)
- Route 53
- Security Group
- EFS

### Other Tools Used:
- DNS resolution
- jdk8
- maven

# Project Architecture on AWS

![](https://github.com/Adutoby/DevOps-Projects-AWS/blob/master/Project-3:%20Lift%20And%20Shift%20Web%20Application%20to%20AWS/images/project%20architecturenew.png)

# Flow of Execution
1. Log into your AWS account
2. Create security groups for the backend services
3. Create key pairs to login into the server
4. Launch EC2 instance with user data (BASH scripts)
5. Update IP to name mapping in Route 53
6. Build our application from source code
7. Upload our application to S3 Bucket
8. Download the artifact to Tomcat EC2 Instance
9. Setup ELB with HTTPS certificate from (ACM) Amazon Certificate Manager
10. Map ELB endpoint to the website name in Amazon Route 53 
11. Configure Auto Scaling Group for the application instance
