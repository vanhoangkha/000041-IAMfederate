---
title : "Federating Azure AD Users to AWS"
date : "`r Sys.Date()`"
weight : 11
chapter : false
pre : " <b> 11. </b> "
---

1. Retrieved from [My Apps](https://myapps.microsoft.com) page

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0001-federatingazureadusers.png)

2. Enter user credentials (eg **```aws-2@firstcloudjourney.onmicrosoft.com```**)
3. Select **Next**

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0002-federatingazureadusers.png)

4. You need to change your password at first login.

5. Then select **Login**

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0003-federatingazureadusers.png)

6. You can see the AWS Single-Account Access App we created. Select to access.

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0004-federatingazureadusers.png)

1. You can now access the AWS Console from Azure AD

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0005-federatingazureadusers.png)

### Check service usage

1. As you know, we assign user aws-2@firstcloudjourney.onmicrosoft.com with S3Full permission.
2. Tried EC2 and we don't have access **You are not authorized to perform this operation**

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0006-federatingazureadusers.png)

3. We can access Amazon S3 through permission setting.

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0007-federatingazureadusers.png)

Congratulations on your successful implementation of Federating from Azure AD.