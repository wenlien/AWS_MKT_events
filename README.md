# Launch free tier EC2 for AWS 2023 MKT event

1. Select a region.

2. Type "EC2" in search bar.

3. Select EC2 service.

4. Click "Launch instance" button.

5. Setup EC2 instance.
   
   1. Input instance name.
      
      E.g. AWS-Training
   
   2. Select Amazon Linux.
   
   3. Choose Amazon Linux 2023 AMI, make sure you see the label of "___Free tier eligible___".
   
   4. Choose t2.micro, make sure you see the label of "___Free tier eligible___".
   
   5. Process without a key pair.
   
   6. Use default VPC/subnet, and also enable "Auto-assign public IP".
      
   7. Create security group.
      
      1. uncheck "Allow SSH traffic from".
      
      2. check "Allow HTTP traffic from the internet".
   
   8. Keep storage as 8GB w/ gp3.
   
   9. Expand "Advanced details" and scroll down to "User data".
      
      1. Copy and paste the following script for user data.
         
         ```shell
         #!/bin/bash
         yum update -y
         yum install -y httpd.x86_64
         systemctl start httpd.service
         systemctl enable httpd.service
         echo "Welcome to AWS Training!!" > /var/www/html/index.html
         ```
   
   10. Review Summary.
   
   11. Click "Launch instace" botton.
   
   12. Click the instance link from the message as below:
       
       E.g. Successfully initiated launch of instance ([i-0fece61c41e7e51b5](https://ap-northeast-2.console.aws.amazon.com/ec2/home?region=ap-northeast-2#Instances:instanceId=i-0fece61c41e7e51b5))
   
   13. Copy "Public IPv4 address" of the instance and paste to the browser.

       Make sure you connect the web server w/ HTTP (___NOT HTTPS___) protocol. (E.g. [http://a.b.c.d](http://a.b.c.d))
   
   14. Verify if you could see the wording from httpd server.
   
   15. Screenshot the EC2 console w/ your id and public ip.
   
   16. Screenshot the web page w/ "Welcom to AWS Training!!".
   
   17. Terminate the EC2 instance.
   
   18. Delete the security group you created.
       
       E.g. launch-wizard-1
   
6. Email two screenshots to [aws_tnc@digitimes.com](mailto:aws_tnc@digitimes.com).

