---
title : "Tạo Identity providers trên AWS"
date :  "`r Sys.Date()`" 
weight : 5
chapter : false
pre : " <b> 5. </b> "
---

1. Đăng nhập vào [AWS Console](https://aws.amazon.com/vi/console/)

![Identity providers](/images/5-Identityproviders/0001-identityprovider.png)

2. Tìm **IAM** và chọn đến giao diện **Identity and Access Management (IAM)**
3. Chọn **Identity providers**

![Identity providers](/images/5-Identityproviders/0002-identityprovider.png)

4. Tạo Identity Provider, chọn **Add provider**

![Identity providers](/images/5-Identityproviders/0003-identityprovider.png)

5. Trong **Add an Identity provider**, phần **Configure provider**

- **Provider type**, chọn **SAML**
- **Provider name**, nhập ```AzureAD```
- **Metadata document**, chọn **Choose file** và upload metadata file **AWS Single-Account Access.xml**

![Identity providers](/images/5-Identityproviders/0004-identityprovider.png)

6. Chọn **Add provider**

![Identity providers](/images/5-Identityproviders/0005-identityprovider.png)

7. Chọn **View provider** để xem chi tiết. 

![Identity providers](/images/5-Identityproviders/0006-identityprovider.png)

8. Chúng ta đã thành công tạo AzureAD Identity Provider trên AWS.

![Identity providers](/images/5-Identityproviders/0007-identityprovider.png)