1. Login Amazon Lex console.

2. Click "Create bot" button.
  <img width="1275" alt="Screenshot 2024-02-16 at 11 41 17 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/e6e3ef0d-2b52-4fef-a613-c61d8d774cc8">

3. Choose "Start with an example", and keep example bot as "BookTrip".
  <img width="1278" alt="Screenshot 2024-02-16 at 11 42 13 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/401862de-7730-4f6c-8507-fb1bb8e8c0da">

4. Give the bot a name as "BookTrip", and provide the description "It's a booking service bot for trip.".
  <img width="803" alt="Screenshot 2024-02-16 at 11 46 31 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/5dd7993a-62bb-4e92-b3e0-9aacaa4d27cf">

5. Choose "Create a role with basic Amazon Lex permissions."
  <img width="804" alt="Screenshot 2024-02-16 at 11 47 35 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/1a41eac0-9599-489f-91a6-ff3490a1c886">

6. Choose "No" for COPPA.
  <img width="804" alt="Screenshot 2024-02-16 at 11 47 59 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/a0a55346-e3cc-4c96-9b18-e7b543657aaf">

7. Remain the existing config and click "Next".
  <img width="807" alt="Screenshot 2024-02-16 at 11 50 45 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/fbbfc599-f774-48c6-8a96-9aa976354694">

8. Remain the existing config and click "Done".
  <img width="1200" alt="Screenshot 2024-02-16 at 11 53 58 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/b286ae1b-c4e7-4bcf-aea3-a6b149c37e3d">

9. Review the configuration of intent and click "Save intent".
  <img width="1274" alt="Screenshot 2024-02-16 at 11 55 16 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/72904f9e-f3a7-4e8a-b5f4-3fbff862d2b6">

10. Click "Build" button on the up left of the page.
  <img width="1276" alt="Screenshot 2024-02-16 at 11 56 00 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/d7da2da0-47fd-48df-9553-58f84467c224">
  <img width="1278" alt="Screenshot 2024-02-16 at 11 56 46 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/6e8b465c-8fa2-45b4-baaf-06d047189278">
  <img width="1280" alt="Screenshot 2024-02-16 at 11 57 26 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/02d9e688-1459-40e4-8e19-473dc1ce1969">

11. Click "Test" button.
  <img width="1279" alt="Screenshot 2024-02-16 at 11 57 47 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/6380c9e0-7710-46c5-80eb-76331bc65709">

12. Input the info of your tip, e.g.
  * Hi
  * Booking a hotel
  * Taipei
  * 2/14
  * 3
  * deluxe
  * yes  
  <img width="349" alt="Screenshot 2024-02-19 at 1 04 25 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/527032af-0dd8-4a7a-b739-ad8489576e25">
  <img width="347" alt="Screenshot 2024-02-19 at 1 05 02 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/3086451f-7ef6-4b27-8b17-d670027435cc">
  <img width="348" alt="Screenshot 2024-02-19 at 1 05 22 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/e14af367-4ea0-4c45-a7fd-52e825f44355">

13. Now, let's customize the dialogue.
  * When we type "Hi", bot replies "Intent FallbackIntent is fulfilled". So, we want bot to understand "Hi".
    * Find "Sample utterances", add "Hi".
    <img width="1277" alt="Screenshot 2024-02-19 at 1 11 30 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/10e55293-f985-4b21-906c-5d1c9f2700e3">
  * To make bot be more friendly, add greeting before process.
    * Find "Initial response", expend "Response to acknowledge the user's request", and type "Hi there, I can help you to book the hotel." in message input box.
    <img width="1278" alt="Screenshot 2024-02-19 at 1 19 25 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/2c558ff4-f1b3-4374-b1e9-75060fc59bc6">
  * To avoid typo by customer, prepare "Room Type" buttons in the dialogue.
    * Expend "Slots", expend "Prompt for slot: RoomType", click "Advanced options".
    <img width="1278" alt="Screenshot 2024-02-19 at 1 43 53 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/5934f81b-fc24-4dc6-ae59-1f3da7c8d211">
    * In pop out screen, find "Slot prompts", expend "Bot elicits information", click "More prompt options".
    <img width="1279" alt="Screenshot 2024-02-19 at 1 28 32 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/cc77ed5f-c995-41e4-aed7-98cd31828121">
    * Expend "Add", and select "Add card group".
    <img width="1277" alt="Screenshot 2024-02-19 at 1 31 41 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/2867ecb3-c80f-41f9-b084-3a9ed7e0ac6e">
    * In "Card1" of Card group, type "Room type" in Title field, and expend "Buttons".
    <img width="1278" alt="Screenshot 2024-02-19 at 1 36 42 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/2cee1fa9-0b80-43cd-beae-fc714f7c001a">
    * Add 3 buttons in "Card 1".

      * Click "Add button" and type "Queen" in title field, "queen" in value field.
      * Click "Add button" and type "King" in title field, "king" in value field.
      * Click "Add button" and type "Deluxe" in title field, "deluxe" in value field.
    <img width="1272" alt="Screenshot 2024-02-19 at 1 40 32 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/9d1a8e65-3e5a-4d35-88b1-6eee85c5a9d6">
    * Click "Update prompts", click "Update slot", then click "Save intent".
    <img width="1278" alt="Screenshot 2024-02-19 at 1 41 48 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/865ebbde-4f9c-4ae3-8b48-d118fdd2a50f">
    <img width="1278" alt="Screenshot 2024-02-19 at 1 45 42 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/7766dc3a-d4d9-4e96-ab79-6dd6cf497303">
  * Click "Build" button on top left of the page, and click "Test" after build success.

    <img width="314" alt="Screenshot 2024-02-19 at 1 54 35 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/2ac1cc19-1316-4a5f-a9ed-cc1fbc738216">
    <img width="316" alt="Screenshot 2024-02-19 at 1 55 00 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/70156abb-b81e-41f8-b49e-70e75090ff46">
    <img width="315" alt="Screenshot 2024-02-19 at 1 55 24 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/5ab3351c-87e1-4a86-be72-84694d7689d5">
    <img width="314" alt="Screenshot 2024-02-19 at 1 55 37 AM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/e4dcbe6a-d606-41ec-aa45-f8b0f2bb3a28">

14. Screenshot your full dialogue with bot (with customized, like above) and also your bot detail information (with your account info, like below).
  <img width="1280" alt="Screenshot 2024-02-16 at 12 07 25 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/d74f3d2e-15ca-4163-835a-eee9da911100">

15. Back to bot page and delete your bot.
  <img width="1281" alt="Screenshot 2024-02-16 at 12 08 55 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/2e9f4e65-94d1-43cb-86d1-147d61d4d927">
  <img width="604" alt="Screenshot 2024-02-16 at 12 11 05 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/fde86c38-383f-4455-9b7d-f5bdac5b3a58">
  <img width="1280" alt="Screenshot 2024-02-16 at 12 11 32 PM" src="https://github.com/wenlien/AWS_MKT_events/assets/348015/23ddb38d-cec6-440d-8093-696e26e7afd8">

16. Email screenshots to aws_tnc@digitimes.com
