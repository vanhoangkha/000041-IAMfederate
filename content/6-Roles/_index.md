---
title : "Create Roles on AWS for Azure AD assume"
date : "`r Sys.Date()`"
weight : 6
chapter : false
pre : " <b> 6. </b> "
---
{{% notice info %}}
In this step we will create 02 roles with access rights as S3 and EC2 to close to the 02 users we created in Azure, **aws-1** and **aws-2**.
{{%/notice%}}

### Create AmazonS3FullAccess

1. Retrieve the IAM Role, select **Role** in the left menu of the AWS IAM service
2. Select **Create role**

![Create IAM Role](/images/6-Roles/0001-createrole.png)

3. In **Trusted entity type**, select **SAML federation**

![Create IAM Role](/images/6-Roles/0002-createrole.png)

4. In **SAML 2.0 federation**
- **SAML 2.0–based provider**, Select the **AzureAD Identity Provider** information we created earlier
- Select **Allow programmatic and AWS Management Console access**
- Then select **Next**


![Create IAM Role](/images/6-Roles/0003-createrole.png)

5. In **Add permissions**, find **AmazonS3FullAccess**

![Create IAM Role](/images/6-Roles/0004-createrole.png)

6. Select **AmazonS3FullAccess**, continue to select **Next**

![Create IAM Role](/images/6-Roles/0005-createrole.png)

7. In **Name, review, and create**

- In the **Role details** section, in the **Role name** section, enter **```S3RoleFull```**

- In the **Description** section, enter **```AmazonS3FullAccess```**

![Create IAM Role](/images/6-Roles/0006-createrole.png)

8. Double check and select **Create role**


![Create IAM Role](/images/6-Roles/0007-createrole.png)

9. Select **View role** to view the details of the newly created role

![Create IAM Role](/images/6-Roles/0008-createrole.png)

10. Role creation results

![Create IAM Role](/images/6-Roles/0009-createrole.png)


### Create AmazonEC2FullAccess


1. Retrieve the IAM Role, select **Role** in the left menu of the AWS IAM service
2. Select **Create role**

![Create IAM Role](/images/6-Roles/0001-createrole.png)

3. In **Trusted entity type**, select **SAML federation**

![Create IAM Role](/images/6-Roles/0002-createrole.png)

4. In **SAML 2.0 federation**
- **SAML 2.0–based provider**, Select the **AzureAD Identity Provider** information we created earlier
- Select **Allow programmatic and AWS Management Console access**
- Then select **Next**


![Create IAM Role](/images/6-Roles/0003-createrole.png)

5. In **Add permissions**, find **AmazonEC2FullAccess**

![Create IAM Role](/images/6-Roles/00010-createrole.png)

6. Select **AmazonEC2FullAccess**, continue to select **Next**

![Create IAM Role](/images/6-Roles/00011-createrole.png)

7. In **Name, review, and create**

- In the **Role details** section, in the **Role name** section, enter **```EC2RoleFull```**

- In the **Description** section, enter **```AmazonEC2FullAccess```**

![Create IAM Role](/images/6-Roles/00012-createrole.png)

8. Double check and select **Create role**


![Create IAM Role](/images/6-Roles/00013-createrole.png)

9. Select **View role** to view the details of the newly created role

![Create IAM Role](/images/6-Roles/00014-createrole.png)

10. Role creation results

![Create IAM Role](/images/6-Roles/00015-createrole.png)