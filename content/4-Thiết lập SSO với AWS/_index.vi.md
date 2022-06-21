---
title : "Thiết lập SSO với AWS"
date :  "`r Sys.Date()`" 
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

1. Trong trang **AWS Single-Account Access**, menu bên trái bạn chọn **Single sign on**

![Thiết lập SSO với AWS](/images/4-SSO/0001-sso.png)

2. Chọn **SAML**

![Thiết lập SSO với AWS](/images/4-SSO/0002-sso.png)

3. Trong phần **Set up Single Sign-On with SAML**

- Mục **Basic SAML Configuration**, chọn **Edit**


![Thiết lập SSO với AWS](/images/4-SSO/0003-sso.png)


4. Mục **Basic SAML Configuration**

- **Identifier (Entity ID)**, thêm **#2** vào đường link để đảm bảo link đăng nhập **SAML** này là duy nhất. Do tài khoản mình đã có một **SAML** trước rồi nên phải sửa link chỗ này.


![Thiết lập SSO với AWS](/images/4-SSO/0004-sso.png)

5. Chọn **Save** để lưu thông tin

![Thiết lập SSO với AWS](/images/4-SSO/0005-sso.png)

6. Các bạn download **Federation Metadata XML**, các bạn sẽ dùng file XML này để upload lên AWS để kết nối.

![Thiết lập SSO với AWS](/images/4-SSO/0006-sso.png)


