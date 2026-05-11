# AWS Portfolio

## Project 1: Static Website using Amazon S3

### Description
I created a static website using Amazon S3 by configuring a bucket for public access and enabling static website hosting.

### AWS Services Used
- Amazon S3
- Bucket Policy
- Static Website Hosting

### Implementation Steps
1. Created an S3 bucket
2. Disabled Block Public Access
3. Uploaded index.html
4. Enabled static website hosting
5. Configured bucket policy to allow public access

### Result
The website is publicly accessible via the S3 website endpoint.

### Challenges
- Invalid bucket policy resource error
- Access issues due to incorrect permissions


## Project 2: Web Server on Amazon EC2

### Description
I deployed a web server on Amazon EC2 by installing Apache and configuring networking to allow public access.

### AWS Services Used
- Amazon EC2
- Security Groups
- Linux (Amazon Linux)
- Apache (httpd)

### Implementation Steps
1. Launched EC2 instance
2. Configured security group (opened ports 22 and 80)
3. Connected via SSH
4. Installed Apache web server
5. Started and enabled the service
6. Created a simple HTML page

### Result
The website is publicly accessible via the EC2 public IP address.

### Challenges
- Failed SSH connection due to port 22 being closed in the Security Group → fixed by allowing SSH access
- Website not accessible due to missing HTTP (port 80) rule → fixed by updating Security Group
  
### Cleanup

- Terminated EC2 instances after testing to avoid unnecessary costs
- Deleted unused EBS volumes
- Ensured no running resources remained

### What I Learned

- How EC2 works as a virtual server
- Importance of Security Groups and ports
- How to install and run a web server (Apache)
- Basic troubleshooting in cloud environments (SSH, networking, service issues)
