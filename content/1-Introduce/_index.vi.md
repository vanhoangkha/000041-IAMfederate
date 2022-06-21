---
title : "Giới thiệu"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

### Tổng quan 

- Mặc định khi bạn tạo tài khoản AWS, bạn cần tạo các tài khoản người dùng (gọi là **IAM Users**) để sử dụng các dịch vụ AWS theo cấp phát, ví dụ **Amazon S3** hay **Amazon EC2**… Các quyền này còn được phân rất cụ thể và tối thiểu (least privilige) theo các action, Region và resource…

- Với một số tổ chức mà users được quản lý ở **Microsoft AD** nhưng vẫn muốn tận dụng danh sách các users này để đăng nhập sử dụng AWS mà không phải tạo thêm các users độc lập theo tổ chức và trên tài khoản AWS. AWS hỗ trợ tính năng này gọi là **IAM Federation**.
  
### Nội dung

{{% notice info %}}
Tạo tài khoản AWS, các bạn tham khảo bài lab [TẠO TÀI KHOẢN AWS ĐẦU TIÊN](https://000001.awsstudygroup.com/vi/)
{{%/notice%}}

1. Tạo tài khoản Azure
2. Khởi tạo Azure Active Directory
3. Tạo Azure AD Users
4. Tạo Enterprise Application
5. Thiết lập SSO
6. Tạo Identity providers
7. Tạo IAM Roles
8. Đồng bộ IAM Roles
9. Provisioning to AWS
10. Federating Azure AD Users truy xuất AWS
11. Federating Azure AD Users đến AWS
12. Dọn dẹp tài nguyên