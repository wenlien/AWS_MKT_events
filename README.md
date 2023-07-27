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
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/e8319480-fc87-4f8a-af4a-11fa9527c6ce">

   
   7. Keep storage as 8GB w/ gp3.
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/a8c80fdf-d184-479e-a3b9-e22f636db6ab">

   
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
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/788db297-cb41-487a-b7d4-f80c32af8298">

   
   9. Review Summary.
   <img width="339" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/c9f91fa9-d8fd-4bd5-8452-fe1303818444">

   
   10. Click "Launch instace" botton.
   
   11. Click the instance link from the message as below:
       
       E.g. Successfully initiated launch of instance (i-0c0e040fded860c1b)
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/c47e8bfd-6a86-491e-85a0-afe3706220d6">

   
   12. Copy "Public IPv4 address" of the instance and paste to the browser.

       Make sure you connect the web server w/ HTTP (___NOT HTTPS___) protocol. (E.g. [http://a.b.c.d](http://a.b.c.d))
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/21bfdc2d-642b-46d5-beca-af79c02ed6fa">

   
   13. Verify if you could see the wording from httpd server.
   
   14. Screenshot the EC2 console w/ your id and public ip.
   
   15. Screenshot the web page w/ "Welcom to AWS Training!!".
   
   16. Terminate the EC2 instance.
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/bde64ddf-da37-40f6-89af-8bfb9e7b515c">

   
   17. Delete the security group you created.
       
       E.g. launch-wizard-1
   <img width="803" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/20ee5f27-691d-4136-99f2-b301af7be287">


6. Email two screenshots to [aws_tnc@digitimes.com](mailto:aws_tnc@digitimes.com).

