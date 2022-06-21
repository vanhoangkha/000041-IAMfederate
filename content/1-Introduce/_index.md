---
title : "Introduction"
date : "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 1. </b> "
---

### Overview

- By default when you create an AWS account, you need to create user accounts (called **IAM Users**) to use provisioned AWS services, for example **Amazon S3** or **Amazon EC2**… These permissions are also very specific and minimal (least privilige) according to actions, Region and resources…

- For some organizations where users are managed at **Microsoft AD** but still want to take advantage of this list of users to log in to use AWS without having to create additional independent users by organization and account AWS. AWS supports this feature called **IAM Federation**.
  
### Content

{{% notice info %}}
Create an AWS account, please refer to the lab [CREATE A FIRST AWS ACCOUNT](https://000001.awsstudygroup.com/en/)
{{%/notice%}}

1. [Create an Azure account]()
2. [Initialize Azure Active Directory]()
3. [Create Azure AD Users]()
4. [Create Enterprise Application]()
5. [Set up SSO]()
6. [Create Identity providers]()
7. [Create IAM Roles]()
8. [Synchronize IAM Roles]()
9. [Provisioning to AWS]()
10. [Federating Azure AD Users accessing AWS]()
11. [Federating Azure AD Users to AWS]()
12. [Clean up resources]()