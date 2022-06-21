---
title : "Dọn dẹp tài nguyên"
date :  "`r Sys.Date()`" 
weight : 12
chapter : false
pre : " <b> 12. </b> "
---

### Xóa Azure AD users

1. Đăng nhập vào trang chủ [Porttal Azure](https://portal.azure.com/#home)
2. Chọn **Azure Active Directory** 
3. Chọn **Users**
4. Trên danh sách user, chọn user cần xóa của bài lab
5. Sau đó chọn **delete user**
6. Chọn **OK**

### Xóa Enterprise applications

1. Đăng nhập vào trang chủ [Porttal Azure](https://portal.azure.com/#home)
2. Chọn **Azure Active Directory**
3. Chọn **Enterprise applications**
4. Chọn **AWS Single-Account Access**
5. Chọn **Properties**
6. Chọn **Delete**
7. Chọn **Yes**

### Xóa tenant

1. Đăng nhập vào trang chủ [Porttal Azure](https://portal.azure.com/#home)
2. Chọn **Azure Active Directory**
3. Trang **Properties**, phần **Access management for Azure resources** chọn **Yes**
4. Chọn **Manage tenants**
5. Chọn **Firstcloudjourney**
6. Chọn **Delete**
7. Sau khi kiểm tra, tiếp tục chọn **Delete**

### Xóa user Identity and Access Management (IAM)

1. Đăng nhập vào [Identity and Access Management (IAM)]()
2. Chọn **Users**
3. Chọn tên user cần xóa của bài lab
4. Chọn **delete**
5. Điền **federating** và chọn **Delete**

### Xóa role Identity and Access Management (IAM)

1. Đăng nhập vào Identity and Access Management (IAM)
2. Chọn **Roles**
3. Chọn **EC2RoleFull** và **S3RoleFull**
4. Sau đó chọn **Delete**
5. Điền vào **delete** 

### Xóa Policies Identity and Access Management (IAM)

1. Đăng nhập vào Identity and Access Management (IAM)
2. Chọn **Policies**
3. Chọn **ListRoles**
4. Chọn **Actions** và chọn **Delete**
5. Điền xác nhận xóa **ListRoles** và chọn **Delete**

### Xóa Identity providers Identity and Access Management (IAM)

1. Đăng nhập vào Identity and Access Management (IAM)
2. Chọn **Identity providers**
3. Chọn **AzureAD**
4. Chọn **Delete**
5. Xác nhận **delete**

