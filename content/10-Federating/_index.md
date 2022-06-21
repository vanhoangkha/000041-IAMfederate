---
title : "Federating Azure AD Users Accessing AWS"
date : "`r Sys.Date()`"
weight : 10
chapter : false
pre : " <b> 10. </b> "
---

1. Assign **Azure AD Users** to **AWS IAM Role**, in Azure AD Portal select **Users and groups**

![Federating Azure AD Users accessing AWS](/images/10-Federating/0001-federating.png)

2. Select **Add user/group**

![Federating Azure AD Users accessing AWS](/images/10-Federating/0002-federating.png)

{{% notice info %}}
Note: For AWS Roles to show up in the next step, you may have to wait 5-10 minutes. And to use the feature of assigning AWS IAM Roles to Azure by Group, you need to upgrade your Azure plan.
{{%/notice%}}

3. In the **Add Assignment** page

- Select **Users**, a list of Users will appear on the right

![Federating Azure AD Users accessing AWS](/images/10-Federating/0003-federating.png)

4. Select the user name (eg **AWScloud-1**) and select **Select**

![Federating Azure AD Users accessing AWS](/images/10-Federating/0004-federating.png)

5. In the **Select a role** section, select **None Select** to select the User Role **AWScloud-1**
6. Select **EC2RoleFull**
7. Select **Select**

![Federating Azure AD Users accessing AWS](/images/10-Federating/0005-federating.png)

8. Select **Assign**

![Federating Azure AD Users accessing AWS](/images/10-Federating/0006-federating.png)

9. You iterate and assign User **AWScloud-2** to **S3RoleFull**.


![Federating Azure AD Users accessing AWS](/images/10-Federating/0007-federating.png)

So you have created a user in Azure AD and connected to AWS through the Identity Provider.