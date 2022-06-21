---
title : "Clean up resources"
date : "`r Sys.Date()`"
weight : 12
chapter : false
pre : " <b> 12. </b> "
---

### Delete Azure AD users

1. Sign in to [Porttal Azure](https://portal.azure.com/#home) homepage
2. Select **Azure Active Directory**
3. Select **Users**
4. On the list of users, select the user to delete from the lab
5. Then select **delete user**
6. Select **OK**

### Delete Enterprise applications

1. Sign in to [Porttal Azure](https://portal.azure.com/#home) homepage
2. Select **Azure Active Directory**
3. Select **Enterprise applications**
4. Select **AWS Single-Account Access**
5. Select **Properties**
6. Select **Delete**
7. Select **Yes**

### Delete tenant

1. Sign in to [Porttal Azure](https://portal.azure.com/#home) homepage
2. Select **Azure Active Directory**
3. On the **Properties** page, in the **Access management for Azure resources** section, select **Yes**
4. Select **Manage tenants**
5. Select **Firstcloudjourney**
6. Select **Delete**
7. After checking, continue to select **Delete**

### Delete User Identity and Access Management (IAM)

1. Log in to [Identity and Access Management (IAM)]()
2. Select **Users**
3. Select the user name to delete the lab
4. Select **delete**
5. Fill in **federating** and select **Delete**

### Remove Identity and Access Management (IAM) role

1. Sign in to Identity and Access Management (IAM)
2. Select **Roles**
3. Select **EC2RoleFull** and **S3RoleFull**
4. Then select **Delete**
5. Fill in **delete**

### Remove Policies Identity and Access Management (IAM)

1. Sign in to Identity and Access Management (IAM)
2. Select **Policies**
3. Select **ListRoles**
4. Select **Actions** and select **Delete**
5. Fill in the deletion confirmation **ListRoles** and select **Delete**

### Delete Identity providers Identity and Access Management (IAM)

1. Sign in to Identity and Access Management (IAM)
2. Select **Identity providers**
3. Select **AzureAD**
4. Select **Delete**
5. Confirm **delete**