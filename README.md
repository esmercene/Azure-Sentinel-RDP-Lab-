# SIEM Lab | Azure Sentinel 

![SIEM Strategy Map](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/5792cec7-a009-43e8-a8ee-fc8099a8c794)

In this SIEM Lab we can use a VM using Microsoft Azure.
First create an Account in Microsoft Azure:
1. Go to the Azure Home Page.https://azure.microsoft.com/en-us/
2. Click on Free Azure Account on the top right corner.

![Screen Shot 2023-10-27 at 2 12 06 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/a4bf26b8-b455-4b04-aa00-15c36d5dba78)
4. Click on Start Free.

![Screen Shot 2023-10-27 at 2 13 27 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/2217d33e-85ef-4208-ba96-619739712146)

4. Sign-in/Sign-up for a Microsoft account using an email address and password.

![Screen Shot 2023-10-27 at 2 15 19 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/58874c02-6c7c-47d7-b92c-0647e98b3883)

5. Enter your Country/Region and Date of Birth and click next.

6. Enter the verification code received on the email address and click next.

7. Type the captcha you see on your screen and click on next.

8. You’ll be redirected to the Azure Sign-up page. Enter your Region, Name, Phone number, Email address. Note: You should use the same email address for Azure sign-up and for the Microsoft account.

9. Verify your phone number by clicking Text Me or Call Me and enter the verification code received.

![Screen Shot 2023-10-27 at 2 17 51 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/8e97644e-d17d-4fe5-86fc-bb0a7ab71cbd)

10. Enter the payment details. Make sure you have a Master Card/American Express/ Visa Credit card and international payments should be enabled.

![Screen Shot 2023-10-27 at 2 19 08 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/4fa6f37e-59eb-4c49-a23c-1cb628b5e6bd)

11. Check the Terms and Conditions and click Sign-up.

![Screen Shot 2023-10-27 at 2 20 25 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/7a09775e-f23c-487c-936c-6942394b5e93)


12. You have successfully created a Microsoft Azure free account and now have a lumpsum balance of $200.

13. Click on Portal on the top right corner of the screen. You’ll be redirected to the Azure portal.

14. If you have exhausted your free credit then you have to move to the Pay as you go subscription policy.

# Create a Virtual Machine

1. Go to https://portal.azure.com/ and go to Virtual Machine, click it or type in the search bar

![Screen Shot 2023-10-27 at 2 27 25 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/b603c86e-7ddc-4e1c-932f-648795cb9efa)

2. Click create Virtual Machine

![Screen Shot 2023-10-27 at 2 30 36 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/62594d8e-6066-4935-a39e-4b843e0c8cf6)

3. Fill-up necessary details to customize as per own preference

![Screen Shot 2023-10-27 at 2 33 37 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/b7a43d9f-8648-4b9f-b44e-a14789f8c77a)

4. In Networking tab click advance and click create new

![Screen Shot 2023-10-27 at 2 35 55 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/10209fa6-2f0d-42dc-82d3-d22c18045a80)

5. Remove all the default and add new inbound rule as below:

![Screen Shot 2023-10-27 at 2 38 38 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/2f429cf0-a326-4cf5-b1ca-b937c7290b6d)

6. Click Review and Create and then on next prompt click Create

![Screen Shot 2023-10-27 at 2 40 33 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/939c8a01-1c34-4305-a622-8eb410147c23)

![Screen Shot 2023-10-27 at 2 40 52 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/b7b12fc6-9a03-4239-b1b1-7e017e886103)

7. While VM is deploying open log analytics workspaces

![Screen Shot 2023-10-27 at 2 43 26 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/265ddc3b-8d20-4c39-a523-1eb709f05294)

8. Create a log analytics workspace

![Screen Shot 2023-10-27 at 2 46 08 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/da47f4b4-b468-4960-bf2a-dadd91550c7e)

![Screen Shot 2023-10-27 at 2 49 40 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/c60ff2ec-78e8-4144-a9b7-8d2b5b5a5fb7)

9. Go to Microsoft Defender for Cloud | Getting started, and click the created log workspace and turn off SQL server machines and click save

![Screen Shot 2023-10-27 at 2 55 11 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/0db906f6-a70e-4f79-bf0b-601dbb81d2ed)

![Screen Shot 2023-10-27 at 2 57 38 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/e65d2963-0c1c-4e0e-b766-ab8abb4b34ed)

10. Go to log analytics workspace, select virtual machine and click connect 

![Screen Shot 2023-10-27 at 3 02 32 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/9cba846f-1e16-47b9-abd4-63c5b72721a0)

![Screen Shot 2023-10-27 at 3 04 09 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/a7c9e865-6989-4b46-932e-beda8f5a3421)

11. Open Virtual Machine and copy the public IP address
12. Open Microsoft Remote Desktop and connect with the public IP and username and password you created
    
![Screen Shot 2023-10-27 at 3 07 54 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/ce97140e-2572-4b2f-9325-1648db9ebbe5)

![Screen Shot 2023-10-27 at 3 11 22 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/75753d96-149b-4215-b65b-0a2da2c44ae8)

![Screen Shot 2023-10-27 at 3 12 19 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/4bc1fdbd-82bb-4699-a175-bb6b617edb94)

13. In your Virtual Machine go to Event Viewer and click Security, and these events are needed to retrieve and pass to Azure Log analytics

![Screen Shot 2023-10-27 at 3 13 58 AM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/68d3d88a-cb18-4dd1-9825-ad5bf2cf1a95)

![Screen Shot 2023-10-27 at 4 50 07 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/b55c6713-d41f-4976-9e06-21f5140fadbb)

14. Create an account with https://ipgeolocation.io/ and get API key to use in PowerShell script included in this repository, replace the API Key in the script with your own API key

![Screen Shot 2023-10-27 at 4 52 17 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/c530ec34-5d9a-4b8e-b8e1-4e3cd2b9fb41)

15. In your VM, open Microsoft Power Shell ISE, copy paste the script and run it.

![Screen Shot 2023-10-27 at 5 06 55 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/dca7f485-af88-46a3-bce3-7cf678924cd0)

16. All Security Log Event will reflect in your ProgramData which you can access through "C:\ProgramData", this is usually hidden (Copy paste this to windows search bar to locate)

![Screen Shot 2023-10-27 at 4 58 08 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/c71bf0d6-b969-47c0-bd4d-645df87d635b)

17. In your Azure go to Log Analytics click Tables and create new custom log and upload the failed_rdp.log from your VM, and name your table you like.

![Screen Shot 2023-10-27 at 5 10 10 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/44b31b1d-1f5b-41c5-a51a-92b0f7f99e2a)

18. Wait for the system to uplaod and reflect the created table, you can check it to Logs. click logs and search for the table you created(e.g. FAILED_RDP_WITH_GEO_CL) then click Run

![Screen Shot 2023-10-27 at 5 15 56 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/de508b12-37b0-400b-8305-110083322995)

19. Now search or go to microsoft Azure Sentinel

![Screen Shot 2023-10-27 at 5 16 58 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/b3ea0e5a-58f0-4215-9b96-95fe67f86cde)

20. Select your created log analytics, select workbook and create new workbook

![Screen Shot 2023-10-27 at 5 20 31 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/a529d62f-d574-45ad-bb1b-c7e44f712a57)

21. Click edit and remove all default settings, and click add to add query as below 

![Screen Shot 2023-10-27 at 5 23 34 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/8cb6462a-6a59-4a6f-8fa7-93831291b445)

22. Run this query, and configure the settings as you like, visualization as Map, click Apply to save all your settings/configurations

`FAILED_RDP_WITH_GEO_CL
| extend RawData = tostring(RawData) 
| parse RawData with * "latitude:" latitude ",longitude:" longitude ",destinationhost:" destinationhost ",username:" username ",sourcehost:" sourcehost ",state:" state ", country:" country ",label:" label ",timestamp:" timestamp
| summarize event_count=count() by sourcehost, latitude, longitude, label, destinationhost, country
| where sourcehost != "" `

![Screen Shot 2023-10-27 at 5 27 22 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/d4f777d8-7b1b-4f94-a65d-ff296485fc77)


23. Click done editing and let it run for a while to retrieve logs of attacks, refresh it to retrieve new log attacks.

![Screen Shot 2023-10-29 at 12 07 25 PM](https://github.com/esmercene/Azure-Sentinel-RDP-Lab-/assets/91687288/63304702-82bf-40f6-8133-5f04343cda7e)


