---
title : "Tạo Azure AD Users"
date :  "`r Sys.Date()`" 
weight : 3
chapter : false
pre : " <b> 2.3 </b> "
---

{{% notice info %}}
Azure AD có tính năng tạo group để quản lý tập users và gán quyền cho group. Việc sử dụng cũng đơn giản nhưng để sử dụng cần upgrade tài khoản Azure nên mình sẽ chỉ hướng dẫn tích hợp phân quyền qua User trong bài lab này.
{{%/notice%}}

### Trong bài lab này, tạo 02 users là **aws-1** và **aws-2**.

1. Chọn **Users**

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0001-createazureadusers.png)

2. Chọn **New user**


![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0002-createazureadusers.png)

3. Trong **Identity** 

- Nhập **User name**. Ví dụ: ```aws-1```
- Nhập **Name**. Ví dụ: ```AWScloud-1```

4. Phần **Password**

- Chọn **Let me create the password**
- **Initial password**, nhập password có độ dài tối thiểu 8 ký tự và các yêu cầu sau:
  - Lowercase characters
  - Uppercase characters
  - Numbers (0-9)
  - Symbols (@ # $ % ^ & * - _ ! + = [ ] { } | \ : ‘ , . ? / ` ~ " ( ) ; < > )
  - Ví dụ: ```Admin@aws123```


![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0003-createazureadusers.png)

5. Các phần còn lại bỏ trống, sau đó chọn **Create**

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0004-createazureadusers.png)

6. Sau khi tạo user, ta có danh sách user sau:

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0005-createazureadusers.png)

7. Chọn tên user và xem chi tiết

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0006-createazureadusers.png)

{{% notice info %}}
Bạn có thể tạo thêm nhiều users để bài labs được nhiều tình huống hơn. 
{{%/notice%}}

8. Thực hiện tạo thêm một user có tên **aws-2**

![Create Azure AD Users](/images/2-Prerequiste/2.3-CreateAzureADUsers/0007-createazureadusers.png)

