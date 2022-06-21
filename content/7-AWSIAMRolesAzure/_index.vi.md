---
title : "Đồng bộ AWS IAM Roles trên AWS qua Azure"
date :  "`r Sys.Date()`" 
weight : 7
chapter : false
pre : " <b> 7. </b> "
---
{{% notice info %}}
Như vậy chúng ta có 02 role trên AWS đã federate đến Azure AD mà chúng ta đã tạo (Firstcloudjourney). Ở bước này, ta đã cấp quyền cho 02 roles nhưng chưa đồng bộ Roles này qua Azure AD.
{{%/notice%}}

Role đã tạo:
- **S3RoleFull** (AmazonS3FullAccess)
- **EC2RoleFull** (AmazonEC2FullAccess)

1. Tạo User Federating Access, mở giao diện **Identity and Access Management (IAM)**
2. Chọn **Users** bên menu trái 
   
![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0001-awsiamrolesazure.png)

3.  Chọn **Add users**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0002-awsiamrolesazure.png)

4. Trong **Add user** 

- **User name**, nhập **```federating```**

5. Trong **Select AWS access type**, chọn **Access key - Programmatic access**

6. Chọn **Next:Permissions**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0003-awsiamrolesazure.png)

7. Chọn **Create policy**


![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0004-awsiamrolesazure.png)


8. Trong **Service** chọn **IAM** 

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0005-awsiamrolesazure.png)

9. Trong **Specify the actions allowed in IAM**, tìm và chọn **ListRoles**

10. Chọn **Next:Tags**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0006-awsiamrolesazure.png)

11. Chọn **Next: Review**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0007-awsiamrolesazure.png)

12. Trong **Review policy** 

- **Name**, nhập **```ListRoles```**
- **Description**, nhập **```ListRoles```**

13. Chọn **Create Policy**


![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0008-awsiamrolesazure.png)


14. Gán **ListRoles** cho User **federating**

- Quay về tab User để tiếp tục chọn Policy cho user **federating** chúng ta đang tạo ở bước trước.
- Chọn **ListRoles**

15. Chọn **Next: Tags**


![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/0009-awsiamrolesazure.png)

16. Chọn  **Next: Review**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/00010-awsiamrolesazure.png)

17. Kiểm tra lại và Chọn **Create user**

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/00011-awsiamrolesazure.png)

18. Tạo user thành công 

![AWS IAM Role Azure](/images/7-AWSIAMRolesAzure/00012-awsiamrolesazure.png)

{{% notice info %}}
Bạn sẽ nhận được Access key ID và Secret access key ở bước này. Chúng ta sẽ dùng Keys này để khai báo bên Azure AD. Các bạn có thể copy key này lại để sử dụng cho bước tiếp theo.
{{%/notice%}}
