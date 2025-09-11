# aws_cloud-practiotioner.md

User data script whenu we add while launching Ec2 then thhat script gets executed when u launch instace and will sshow you that output when u start server
ex - code of user data is given in zip

#!/bin/bash
# Use this for your user data (script from top to bottom)
# install httpd (Linux 2 version)
yum update -y
yum install -y httpd
systemctl start httpd
systemctl enable httpd
echo "<h1>Hello World from $(hostname -f)</h1>" > /var/www/html/index.html

with this user data script u wiull see output hello world from IP when u visite IP
