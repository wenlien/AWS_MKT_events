# Launch free tier SageMaker for AWS 2023 MKT event

1. Select a region.

2. Type "SageMaker" in search bar.
   <img width="940" alt="Screenshot 2024-02-13 at 1 10 33 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/db66891a-e652-4f64-bccc-7cc219781de4">

3. Select SageMaker service.

4. Expense "Notebook" in left side bar.

5. Click "Notebook Instances" link.

6. Click "Create notebook instance" button.
   <img width="992" alt="Screenshot 2024-02-13 at 1 16 53 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/6ae4062f-0746-4387-82a2-31f02cd69bfe">

7. Setup SageMaker notebook instance.
   
   1. Input instance name.

      E.g. AWS-Training
   <img width="803" alt="Screenshot 2024-02-13 at 1 21 46 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/2d8ce196-4c52-4ba6-a50e-aac0d4e2d1ac">
   
   2. In permissions and encryption block, expend the "IAM role" and select "create a new role".
   <img width="803" alt="Screenshot 2024-02-13 at 1 27 46 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/ad6dcfe1-8d0f-442b-8ddc-9501b4c62286">

   3. Click "Create Role".
   <img width="824" alt="Screenshot 2024-02-13 at 1 31 08 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/60ba508b-df72-45e7-bacb-0910c9cec7c1">

   4. Then you will get a notification about role was created.
   <img width="763" alt="Screenshot 2024-02-13 at 1 26 41 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/26cfcf00-996b-4537-a3e6-05962476c9c3">

   5. Click "Create notebook instance".
   <img width="806" alt="Screenshot 2024-02-13 at 1 37 29 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/8c8d6721-e6de-4eff-8da2-23ad7dbf8924">

   6. You will get a notification about "Success! Your notebook instance is being created."
   <img width="997" alt="Screenshot 2024-02-13 at 1 38 13 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/46a5fa67-f367-469b-aedd-3637ee76a19b">

   
   5. Use default VPC, subnet w/ auto-assign public IP enabled, and also enable "Auto-assign public IP".
      
   6. Create security group.
      
      1. uncheck "Allow SSH traffic from".
      
      2. check "Allow HTTP traffic from the internet".
   <img width="800" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/e8319480-fc87-4f8a-af4a-11fa9527c6ce">
   
   16. Terminate the SageMaker notebook instance.
   <img width="800" alt="image" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/bde64ddf-da37-40f6-89af-8bfb9e7b515c">


8. Email two screenshots to [aws_tnc@digitimes.com](mailto:aws_tnc@digitimes.com)

