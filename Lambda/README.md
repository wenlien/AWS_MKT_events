1. Login to AWS Lambda console.
<img width="1281" alt="Screenshot 2024-02-27 at 12 00 23 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/010b2fd0-951d-48c0-9430-df96971b381a">

2. Select "Use a blueprint".
<img width="1282" alt="Screenshot 2024-02-27 at 12 01 05 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/9e6c5f6c-9fe1-4eff-8413-2ff2ef9d79d1">

3. Expend drop down list of Blueprint name, and select "Getting started with Lambda HTTP".
<img width="826" alt="Screenshot 2024-02-27 at 4 16 05 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/3ce2a82e-41b3-4cf9-a4ec-558b3afea77f">

4. Give Lambda function a name, e.g. "AWS-Training".
<img width="1137" alt="Screenshot 2024-02-27 at 4 16 53 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/e5ae1d26-d8fe-44f8-86cc-bba432f07e28">

5. Review the source code of Lambda function.
<img width="1144" alt="Screenshot 2024-02-27 at 4 17 15 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/67faa44a-71ef-4213-9bc9-c77a4c943398">

6. Check "Acknowledgement" for enable open policy for Lambda function URL, and click "Create function" button.
<img width="1211" alt="Screenshot 2024-02-27 at 4 33 27 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/08164ae4-56ad-45a8-800d-4715d194c95b">

7. Wait for few seconds and you will be noticed that Lambda function has been created successfully, and click "Function URL" hyperlink to browse the web page.
<img width="1284" alt="Screenshot 2024-02-27 at 4 20 01 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/5c3c40fa-0b82-4d73-a753-da1bb423f91a">

8. You will the page with the wording "Hello from AWS Lambda!".
<img width="1282" alt="Screenshot 2024-02-27 at 4 20 27 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/20f2c1a8-ef64-4ec4-944d-fd457d1a0472">

9. Now, we'll try to modify the page, click index.html in the left side bar.
<img width="1210" alt="Screenshot 2024-02-27 at 4 22 08 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/9835dbac-c800-49c6-95ce-e0bf531828f0">

10. Find the phrase "Hello from AWS Lambda!" (2 places) and replace them by "Hello, AWS Training!".
<img width="1282" alt="Screenshot 2024-02-27 at 4 22 29 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/6af82acc-599d-4924-bd73-7858dc6b939d">

11. After modification, you will see the label "Changes not deployed" next to the button "Deploy".
<img width="1282" alt="Screenshot 2024-02-27 at 4 24 03 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/75f0bd69-5f28-43ba-bce1-01feb5380c98">

12. Click the "Deploy" button and refresh the page, then you will see the new wording "Hello, AWS Training".
<img width="1279" alt="Screenshot 2024-02-27 at 4 24 23 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/92b14d5c-a96f-40f1-84e3-fb1b211175e7">

13. To avoid addtional billing, we're going to delete the Lambda fuction.  But, before you delete the Lambda function, you need to take two screenshot first.

14. Search Lambda function by input filter "AWS-Training".
<img width="1281" alt="Screenshot 2024-02-27 at 4 25 07 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/0d1d9f85-3b3c-44b6-a2dd-799503364927">

15. Check Lambda function "AWS-Training", and select "Delete" from "Action" drop down list.
<img width="1281" alt="Screenshot 2024-02-27 at 4 25 21 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/38c467c1-addb-40c7-b688-2526af95c37b">

16. Type "delete" to confirm deletion, and clikc "Delete" button.
<img width="743" alt="Screenshot 2024-02-27 at 4 25 35 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/fe847400-1038-41a8-9597-7ee2add6551b">

17. Verify you Lambda function has been deleted.
<img width="1281" alt="Screenshot 2024-02-27 at 4 25 56 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/130464fa-cf53-4bfe-bb23-79bf75dca1d9">
