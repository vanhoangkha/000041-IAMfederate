---
title : "Tạo Roles trên AWS để Azure AD assume"
date :  "`r Sys.Date()`" 
weight : 6
chapter : false
pre : " <b> 6. </b> "
---
{{% notice info %}}
Ở bước này chúng ta sẽ tạo 02 roles với quyền truy xuất là S3 và EC2 để gấn cho 02 users chúng ta đã tạo ở Azure là **aws-1** và **aws-2**.
{{%/notice%}}

### Tạo AmazonS3FullAccess

1. Truy xuất IAM Role, chọn **Role** ở menu bên trái của dịch vụ AWS IAM
2. Chọn **Create role**

![Create IAM Role](/images/6-Roles/0001-createrole.png)

3. Trong **Trusted entity type**, chọn **SAML federation**

![Create IAM Role](/images/6-Roles/0002-createrole.png)

4. Trong **SAML 2.0 federation** 
- **SAML 2.0–based provider**, Chọn thông tin **AzureAD Identity Provider** chúng ta đã tạo từ trước
- Chọn **Allow programmatic and AWS Management Console access**
- Sau đó chọn **Next**


![Create IAM Role](/images/6-Roles/0003-createrole.png)

5. Trong **Add permissions**, tìm **AmazonS3FullAccess**

![Create IAM Role](/images/6-Roles/0004-createrole.png)

6. Chọn **AmazonS3FullAccess**, tiếp tục chọn **Next**

![Create IAM Role](/images/6-Roles/0005-createrole.png)

7. Trong **Name, review, and create**

- Phần **Role details**, mục **Role name**, nhập **```S3RoleFull```**

- Phần **Description**, nhập **```AmazonS3FullAccess```**

![Create IAM Role](/images/6-Roles/0006-createrole.png)

8. Kiểm tra lại và chọn **Create role**


![Create IAM Role](/images/6-Roles/0007-createrole.png)

9. Chọn **View role** để xem chi tiết role vừa tạo

![Create IAM Role](/images/6-Roles/0008-createrole.png)

10. Kết quả tạo role

![Create IAM Role](/images/6-Roles/0009-createrole.png)

### Tạo AmazonEC2FullAccess


1. Truy xuất IAM Role, chọn **Role** ở menu bên trái của dịch vụ AWS IAM
2. Chọn **Create role**

![Create IAM Role](/images/6-Roles/0001-createrole.png)

3. Trong **Trusted entity type**, chọn **SAML federation**

![Create IAM Role](/images/6-Roles/0002-createrole.png)

4. Trong **SAML 2.0 federation** 
- **SAML 2.0–based provider**, Chọn thông tin **AzureAD Identity Provider** chúng ta đã tạo từ trước
- Chọn **Allow programmatic and AWS Management Console access**
- Sau đó chọn **Next**


![Create IAM Role](/images/6-Roles/0003-createrole.png)

5. Trong **Add permissions**, tìm **AmazonEC2FullAccess**

![Create IAM Role](/images/6-Roles/00010-createrole.png)

6. Chọn **AmazonEC2FullAccess**, tiếp tục chọn **Next**

![Create IAM Role](/images/6-Roles/00011-createrole.png)

7. Trong **Name, review, and create**

- Phần **Role details**, mục **Role name**, nhập **```EC2RoleFull```**

- Phần **Description**, nhập **```AmazonEC2FullAccess```**

![Create IAM Role](/images/6-Roles/00012-createrole.png)

8. Kiểm tra lại và chọn **Create role**


![Create IAM Role](/images/6-Roles/00013-createrole.png)

9. Chọn **View role** để xem chi tiết role vừa tạo

![Create IAM Role](/images/6-Roles/00014-createrole.png)

10. Kết quả tạo role

![Create IAM Role](/images/6-Roles/00015-createrole.png)


