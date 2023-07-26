# Launch free tier EC2 for MKT event

1. Choose a region

2. Type "EC2" in search bar

3. Select EC2 service

4. Click "Launch instance" botton

5. Setup EC2 instance
   
   1. Input Name, e.g. AWS-Training
   
   2. Select Amazon Linux
   
   3. Choose Amazon Linux 2023 AMI, make sure you see the label <Free tier eligible>
   
   4. Choose t2.micro, make sure you see the label <Free tier eligible>
   
   5. Process without a key pair
   
   6. Create security group
      
      1. uncheck "Allow SSH traffic from"
      
      2. check "Allow HTTP traffic from the internet"
   
   7. Keep storage as 8GB w/ gp3
   
   8. Expand "Advanced details" and scroll down to "User data"
      
      1. Copy and paste the following script for user data
         
         ```shell
         #!/bin/bash
         yum update -y
         yum install -y httpd.x86_64
         systemctl start httpd.service
         systemctl enable httpd.service
         echo "Welcome to AWS Training!!" > /var/www/html/index.html
         ```
   
   9. Review Summary
   
   10. Click "Launch instace" botton
   
   11. Click the instance link from the message as below:
       E.g. Successfully initiated launch of instance ([i-0fece61c41e7e51b5](https://ap-northeast-2.console.aws.amazon.com/ec2/home?region=ap-northeast-2#Instances:instanceId=i-0fece61c41e7e51b5))
   
   12. Copy "Public IPv4 address" of the instance and paste to the browser
   
   13. Verify if you could see the wording from httpd server.
   
   14. Screenshot the EC2 console w/ your id and public ip.
   
   15. Screenshot the web page w/ "Welcom to AWS Training!!".
   
   16. Terminate the EC2 instance.
   
   17. Delete the security group you created.
       E.g. launch-wizard-1
   
   18. email two screenshots to [aws_tnc@digitimes.com](mailto:aws_tnc@digitimes.com)
