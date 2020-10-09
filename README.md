# outlinetemplate--quickstart
   this repo is used to guide you quick setup a outline environment in Azure by ARM template. Please go through the Readme document's setup guide part step by step. Enjoy it!  
   
## Setup Guide
1. Prepare your user managed identity, which will be used in the deployment process.

   a. Sign in to the Azure portal using an account associated with the Azure subscription to create the user-assigned managed identity.

   b. In the search box, type Managed Identities, and under Services, click Managed Identities.
   
   c. Click Add and enter values in the following fields under Create user assigned managed identity pane:
   
       Subscription: Choose the subscription to create the user-assigned managed identity under.
       
       Resource group: Choose a resource group to create the user-assigned managed identity in or click Create new to create a new resource group.
       
       Region: Choose a region to deploy the user-assigned managed identity, for example SouthEast Asia.
       
       Name: This is the name for your user-assigned managed identity, for example outlinemsi.
       
   ![Deploy To Azure](https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/media/how-to-manage-ua-identity-portal/create-user-assigned-managed-identity-portal.png)
   
   d. Assign the created Managed Identity above with subscription owner priviledge. In the search box, type Subscriptions, select the available subscription, then select Access control(IAM), select Add role assignment to assign the OWNER role to the Managed Identity.
       
       
2. click the deploy to azure icon below, start the automatic deployment process.
   
   [![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fnonokangwei%2Foutlinetemplate%2Fmain%2Ftemplate-with-inlinescript%2Foutline_arm_inlinescript.json)
   
   a. Set the region as southeast asia or east asia.
   
   b. Select Location with southeastasia or eastasia.
   
   c. Set the outline vm's admin password. For example, Outline!123.
   
   d. Set the Identity as the ID you collect in Step 1.

3. setup outline client on your mobile phone.

   a. Android client download from [here](https://github.com/Jigsaw-Code/outline-client/releases/download/android-v1.4.0/android-v1.4.0.apk).
   
   b. IPhone client download directly from app store, app name is outline.
   
4. config the outline client
   
   copy the output connection string to the client. For example, connection string pattern: ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTppUVFrS1NHRXdCOEE=@x.x.x.x:54623/?outline=1
