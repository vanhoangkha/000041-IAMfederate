---
title : "Sync AWS IAM Roles on AWS via Azure"
date : "`r Sys.Date()`"
weight : 7
chapter : false
pre : " <b> 7. </b> "
---
{{% notice info %}}
So we have 02 roles on AWS federate to the Azure AD we created (Firstcloudjourney). In this step, we have granted permission to 02 roles but have not synced these Roles through Azure AD.
{{%/notice%}}

Roles created:
- **S3RoleFull** (AmazonS3FullAccess)
- **EC2RoleFull** (AmazonEC2FullAccess)

1. Create User Federating Access, open **Identity and Access Management (IAM)** interface
2. Select **Users** on the left menu
   
![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0001-awsiamrolesazure.png)

3. Select **Add users**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0002-awsiamrolesazure.png)

4. In **Add user**

- **User name**, enter **```federating```**

5. In **Select AWS access type**, select **Access key - Programmatic access**

6. Select **Next:Permissions**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0003-awsiamrolesazure.png)

7. Select **Create policy**


![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0004-awsiamrolesazure.png)


8. In **Service** select **IAM**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0005-awsiamrolesazure.png)

9. In **Specify the actions allowed in IAM**, find and select **ListRoles**

10. Select **Next:Tags**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0006-awsiamrolesazure.png)

11. Select **Next: Review**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0007-awsiamrolesazure.png)

12. In **Review policy**

- **Name**, enter **```ListRoles```**
- **Description**, enter **```ListRoles```**

13. Select **Create Policy**


![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0008-awsiamrolesazure.png)


14. Assign **ListRoles** to User **federating**

- Go back to the User tab to continue selecting the Policy for the **federating** user we were creating in the previous step.
- Select **ListRoles**

15. Select **Next: Tags**


![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0009-awsiamrolesazure.png)

16. Select **Next: Review**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/00010-awsiamrolesazure.png)

17. Check again and Select **Create user**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/00011-awsiamrolesazure.png)

18. Create a successful user

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/00012-awsiamrolesazure.png)

{{% notice info %}}
You will get the Access key ID and Secret access key in this step. We will use this Keys to declare in Azure AD. You can copy this key to use for the next step.
{{%/notice%}}