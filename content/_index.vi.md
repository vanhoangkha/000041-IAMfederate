---
title : "AWS IAM Federation từ Microsoft Azure Active Directory"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
---
# AWS IAM Federation từ Microsoft Azure Active Directory

### Tổng quan

Ở bài lab này chúng ta sẽ cùng nhau tìm hiểu tính năng IAM Federation trên AWS. Một khái niệm trừu tượng với những bạn mới bắt đầu tìm hiểu về AWS. 

Kết quả của bài lab này:

1. Tích hợp Microsoft Azure AD với IAM thông qua SAML

2. User tạo trên Microsoft Azure AD có khả năng kết nối vào AWS để sử dụng các quyền hạn theo thiết lập ở cả hai phía AWS và Azure.

3. Hiểu về IAM Federation

### Khái niệm về SAML

- SAML là viết tắt của **Security Assertion Markup language**(ngôn ngữ Đánh dấu xác nhận bảo mật).
- Nói chung, người dùng cần nhập tên người dùng và mật khẩu để đăng nhập vào bất kỳ ứng dụng nào.
- SAML là một kỹ thuật đạt được **Single Sign-On** – Đăng nhập một lần (SSO) .
- **Security Assertion Markup Language** (SAML) là một khuôn khổ dựa trên Xml cho phép nhà cung cấp danh tính cung cấp thông tin xác thực ủy quyền cho nhà cung cấp dịch vụ.
- Với SAML, bạn cần nhập một thuộc tính bảo mật để đăng nhập vào ứng dụng
- SAML là liên kết giữa xác thực danh tính của người dùng và ủy quyền sử dụng dịch vụ.
- SAML cung cấp một dịch vụ được gọi là Đăng nhập một lần có nghĩa là người dùng phải đăng nhập một lần và có thể sử dụng cùng thông tin xác thực để đăng nhập vào nhà cung cấp dịch vụ khác. 
  
### Nội dung

1. [Giới thiệu]()
2. [Các bước chuẩn bị]()
3. [Khởi tạo Azure AD]()
4. [Tạo Azure AD Users]()
5. [Tạo Enterprise Application (EA) kết nối AWS]()
6. [Thiết lập SSO với AWS]()
7. [Tạo Identity Provider trên AWS]()
8. [Đồng bộ Roles trên AWS để Azure AD assume]()
9. [Federating Azure AD Users truy xuất AWS]()
10. [Federating Azure AD Users đến AWS]()
11. [Kiểm tra dịch vụ sử dụng]()