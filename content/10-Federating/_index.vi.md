---
title : "Federating Azure AD Users truy xuất AWS"
date :  "`r Sys.Date()`" 
weight : 10
chapter : false
pre : " <b> 10. </b> "
---

1. Gán **Azure AD Users** vào **AWS IAM Role**, trong Azure AD Portal chọn **Users and groups**

![Federating Azure AD Users truy xuất AWS](/images/10-Federating/0001-federating.png)

2. Chọn **Add user/group**

![Federating Azure AD Users truy xuất AWS](/images/10-Federating/0002-federating.png)

{{% notice info %}}
Lưu ý: Để Roles bên AWS hiện thị ở bước tiếp theo bạn có thể phải chờ 5-10 phút nhé. Và để sử dụng tính năng gán AWS IAM Role cho Azure theo Group bạn cần nâng cấp plan sử dụng Azure.
{{%/notice%}}

3. Trong trang **Add Assignment**

- Chọn **Users**, xuất hiện danh sách User bên phải 

![Federating Azure AD Users truy xuất AWS](/images/10-Federating/0003-federating.png)

4. Chọn tên user (ví dụ: **AWScloud-1**) và chọn **Select**

![Federating Azure AD Users truy xuất AWS](/images/10-Federating/0004-federating.png)

5. Phần **Select a role**, chọn **None Select** để lựa chọn Role của User **AWScloud-1**
6. Chọn **EC2RoleFull** 
7. Chọn **Select** 

![Federating Azure AD Users truy xuất AWS](/images/10-Federating/0005-federating.png)

8. Chọn **Assign**

![Federating Azure AD Users truy xuất AWS](/images/10-Federating/0006-federating.png)

9. Bạn lặp lại và gán User **AWScloud-2** cho **S3RoleFull**.


![Federating Azure AD Users truy xuất AWS](/images/10-Federating/0007-federating.png)

Vậy là bạn đã thực hiện tạo user bên Azure AD và kết nối đến AWS thông qua Identity Provider.
