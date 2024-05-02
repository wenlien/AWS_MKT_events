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
   
   2. In permissions and encryption block, expend the "IAM role" and select "Create a new role".
   <img width="803" alt="Screenshot 2024-02-13 at 1 27 46 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/ad6dcfe1-8d0f-442b-8ddc-9501b4c62286">

   3. Click "Create Role".
   <img width="824" alt="Screenshot 2024-02-13 at 1 31 08 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/60ba508b-df72-45e7-bacb-0910c9cec7c1">

   4. Then you will get a notification about role was created.
   <img width="763" alt="Screenshot 2024-02-13 at 1 26 41 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/26cfcf00-996b-4537-a3e6-05962476c9c3">

   5. Click "Create notebook instance".
   <img width="806" alt="Screenshot 2024-02-13 at 1 37 29 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/8c8d6721-e6de-4eff-8da2-23ad7dbf8924">

   6. You will get a notification about "Success! Your notebook instance is being created."
   <img width="997" alt="Screenshot 2024-02-13 at 1 38 13 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/46a5fa67-f367-469b-aedd-3637ee76a19b">

   7. Launch Jupyter notebook UI by clicking the link of "Open Jupyter".
   <img width="996" alt="Screenshot 2024-02-13 at 1 01 24 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/d736f031-228b-40e0-8924-9a08fb73a196">

   8. Download notebook file and data from github.
      
      * [AWS_MKT_Events_SageMaker.ipynb](https://github.com/wenlien/AWS_MKT_events/blob/main/SageMaker/AWS_MKT_Events_SageMaker.ipynb)
   
      * [students.csv](https://github.com/wenlien/AWS_MKT_events/blob/main/SageMaker/students.csv)
   
   9. Upload notebook file and data to SageMaker notebook instance by clicking "Upload" button at the up right of the page.
   
   <img width="1267" alt="Screenshot 2024-02-14 at 8 10 30 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/d4d10855-1acf-436a-b96c-9baf4b368866">

   <img width="1278" alt="Screenshot 2024-02-14 at 8 13 57 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/1466c610-aeac-4b17-9974-4f3027329be5">

   <img width="1275" alt="Screenshot 2024-02-14 at 8 14 19 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/95bf6b06-5956-41cf-a8b5-efd0213b0d51">

   10. Click "AWS_MKT_Events_SageMaker.ipynb" to open the script.

   <img width="1277" alt="Screenshot 2024-02-14 at 10 43 22 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/bae3df8d-437f-4696-bfdd-0abbbb233c34">

   11. Make sure the current kernel of the notebook is "conda_python3" or change the kernel by clicking "Kernel" -> "Change kernel" -> "conda_python3"

   <img width="1278" alt="Screenshot 2024-02-14 at 10 44 07 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/bb672341-0c3b-490a-856a-6bb8f4a9522b">

   12. Run each cell and get the result.

   13. Take two screenshots for your environment.
       
      * Click your notebook instance, and screenshot the detail info of your server and also your account.
   <img width="1281" alt="3_Screenshot 2024-02-27 at 5 36 39 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/eb3a1c7e-4c5f-4d78-9340-145d1912ffc2">

      * Screenshot the last cell (bar chart) output of notebook.
   <img width="1278" alt="Screenshot 2024-02-14 at 10 54 11 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/19197554-b271-4a48-a6de-0c32a197f784">

   14. Stop the SageMaker notebook instance.

   <img width="1280" alt="Screenshot 2024-02-14 at 11 03 08 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/4a35d9d9-ae97-4c29-8083-299ebe69d059">

   15. Terminate the SageMaker notebook instance after it stopped.
   
   <img width="1280" alt="Screenshot 2024-02-14 at 11 06 11 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/3e78beda-d8cf-488b-8fe4-be51fcbbc0aa">


9. Email two screenshots to [aws_tnc@digitimes.com](mailto:aws_tnc@digitimes.com)

