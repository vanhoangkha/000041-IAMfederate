---
title : "Create Azure AD Users"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 2.3 </b> "
---

{{% notice info %}}
Azure AD has a group creation feature to manage the set of users and assign permissions to the group. The use is also simple, but to use it, it is necessary to upgrade the Azure account, so I will only guide the integration of authorization via User in this lab.
{{%/notice%}}

### In this lab, create 02 users **aws-1** and **aws-2**.

1. Select **Users**

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0001-createazureadusers.png)

2. Select **New user**


![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0002-createazureadusers.png)

3. In **Identity**

- Enter **User name**. Example: ```aws-1```
- Enter **Name**. Example: ```AWScloud-1```

4. **Password** section

- Select **Let me create the password**
- **Initial password**, enter a password with a minimum length of 8 characters and the following requirements:
  - Lowercase characters
  - Uppercase characters
  - Numbers (0-9)
  - Symbols (@ # $ % ^ & * - _ ! + = [ ] { } | \ : ' , . ? / ` ~ " ( ) ; < > )
  - Example: ```Admin@aws123```


![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0003-createazureadusers.png)

5. Leave the rest blank, then select **Create**

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0004-createazureadusers.png)

6. After creating the user, we have the following list of users:

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0005-createazureadusers.png)

7. Select user name and view details

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0006-createazureadusers.png)

{{% notice info %}}
You can create more users to give labs more scenarios.
{{%/notice%}}

8. Create a new user named **aws-2**

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0007-createazureadusers.png)