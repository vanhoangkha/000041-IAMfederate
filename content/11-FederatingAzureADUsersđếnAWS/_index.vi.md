---
title : "Federating Azure AD Users đến AWS"
date :  "`r Sys.Date()`" 
weight : 11
chapter : false
pre : " <b> 11. </b> "
---

1. Truy xuất từ trang [My Apps](https://myapps.microsoft.com)

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0001-federatingazureadusers.png)

2. Nhập thông tin đăng nhập user (ví dụ: **```aws-2@firstcloudjourney.onmicrosoft.com```**)
3. Chọn **Tiếp theo**

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0002-federatingazureadusers.png)

4. Bạn cần phải thay đổi mật khẩu ở lần đăng nhập đầu tiên. 

5. Sau đó chọn **Đăng nhập**

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0003-federatingazureadusers.png)

6. Các bạn có thể thấy AWS Single-Account Access App mà chúng ta đã tạo. Chọn để truy xuất nhé.

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0004-federatingazureadusers.png)

7. Bạn đã có thể truy xuất AWS Console từ Azure AD

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0005-federatingazureadusers.png)

### Kiểm tra dịch vụ sử dụng

1. Như các bạn đã biết, chúng ta gán user aws-2@firstcloudjourney.onmicrosoft.com với quyền S3Full.
2. Thử EC2 và chúng ta ko có quyền truy xuất **You are not authorized to perform this operation**

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0006-federatingazureadusers.png)

3. Chúng ta có thể truy xuất Amazon S3 thông qua thiết lập quyền.

![Federating Azure AD Users đến AWS](/images/11-FederatingAzureADUsersđếnAWS/0007-federatingazureadusers.png)

Chúc mừng các bạn đã thành công thực hiện Federating từ Azure AD.


