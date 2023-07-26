# Launch free tier EC2 for AWS 2023 MKT event

1. Select a region.

2. Type "EC2" in search bar.

3. Select EC2 service.

4. Click "Launch instance" button.

5. Setup EC2 instance.
   
   1. Input instance name.
      
      E.g. AWS-Training
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/33287738-c40e-4ae9-bd7c-f26f915aff1c">

   
   2. Select Amazon Linux and choose Amazon Linux 2023 AMI, make sure you see the label of "___Free tier eligible___".
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/8005d475-c677-4639-8356-fc5eaf246bf2">

   
   3. Choose t2.micro, make sure you see the label of "___Free tier eligible___".
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/ca5bb0cc-b658-4f64-9992-0216d3260fbf">

   
   4. Process without a key pair.
   <img width="802" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/d40e7afa-2218-40e3-96b0-52ceec9d0620">

   
   5. Use default VPC, subnet w/ auto-assign public IP enabled, and also enable "Auto-assign public IP".
      
   6. Create security group.
      
      1. uncheck "Allow SSH traffic from".
      
      2. check "Allow HTTP traffic from the internet".
   <img width="703" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/e8319480-fc87-4f8a-af4a-11fa9527c6ce">

   
   7. Keep storage as 8GB w/ gp3.
   <img width="702" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/a8c80fdf-d184-479e-a3b9-e22f636db6ab">

   
   8. Expand "Advanced details" and scroll down to "User data".
      
      1. Copy and paste the following script for user data.
         
         ```shell
         #!/bin/bash
         yum update -y
         yum install -y httpd.x86_64
         systemctl start httpd.service
         systemctl enable httpd.service
         echo "Welcome to AWS Training!!" > /var/www/html/index.html
         ```
   
   9. Review Summary.
   
   10. Click "Launch instace" botton.
   
   11. Click the instance link from the message as below:
       
       E.g. Successfully initiated launch of instance ([i-0fece61c41e7e51b5](https://ap-northeast-2.console.aws.amazon.com/ec2/home?region=ap-northeast-2#Instances:instanceId=i-0fece61c41e7e51b5))
   
   12. Copy "Public IPv4 address" of the instance and paste to the browser.

       Make sure you connect the web server w/ HTTP (___NOT HTTPS___) protocol. (E.g. [http://a.b.c.d](http://a.b.c.d))
   
   13. Verify if you could see the wording from httpd server.
   
   14. Screenshot the EC2 console w/ your id and public ip.
   
   15. Screenshot the web page w/ "Welcom to AWS Training!!".
   
   16. Terminate the EC2 instance.
   
   17. Delete the security group you created.
       
       E.g. launch-wizard-1
   
6. Email two screenshots to [aws_tnc@digitimes.com](mailto:aws_tnc@digitimes.com).

