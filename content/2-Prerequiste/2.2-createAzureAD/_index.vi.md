---
title : "Khởi tạo Azure Active Directory "
date :  "`r Sys.Date()`" 
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---

### Tổng quan 

**Azure Active Directory (Azure AD)** là một dịch vụ quản lý truy cập và nhận dạng dựa trên đám mây. Dịch vụ này giúp bạn truy cập các tài nguyên bên ngoài, chẳng hạn như Microsoft 365, cổng Azure và hàng nghìn ứng dụng SaaS khác. Azure AD cũng giúp họ truy cập tài nguyên bên trong. Đây là những tài nguyên như ứng dụng trên mạng công ty và mạng nội bộ của bạn, cùng với bất kỳ ứng dụng đám mây nào do tổ chức của bạn phát triển

### Người dùng Azure AD

- **Quản trị viên CNTT**: sử dụng Azure AD để kiểm soát quyền truy cập vào ứng dụng và tài nguyên ứng dụng của bạn, dựa trên yêu cầu kinh doanh của bạn. Ví dụ: bạn có thể sử dụng Azure AD để yêu cầu xác thực đa yếu tố khi truy cập các tài nguyên quan trọng của tổ chức. Bạn cũng có thể sử dụng Azure AD để tự động cấp phép người dùng giữa Windows Server AD hiện có và các ứng dụng đám mây của bạn, bao gồm cả **Microsoft 365**. Azure AD cung cấp cho bạn các công cụ mạnh mẽ để tự động giúp bảo vệ danh tính và thông tin xác thực của người dùng cũng như đáp ứng các yêu cầu quản trị quyền truy cập của bạn.
- **Nhà phát triển ứng dụng**: sử dụng Azure AD làm phương pháp tiếp cận dựa trên tiêu chuẩn để thêm đăng nhập một lần (SSO) vào ứng dụng của bạn, cho phép ứng dụng hoạt động với thông tin đăng nhập sẵn có của người dùng. Azure AD cũng cung cấp các API có thể giúp bạn xây dựng trải nghiệm ứng dụng được cá nhân hóa bằng cách sử dụng dữ liệu tổ chức hiện có. 
- **Người đăng ký Microsoft 365, Office 365, Azure hoặc Dynamics CRM Online**: Mỗi đối tượng thuê Microsoft 365, Office 365, Azure và Dynamics CRM Online tự động là đối tượng thuê Azure AD. Bạn có thể bắt đầu ngay lập tức để quản lý quyền truy cập vào các ứng dụng đám mây tích hợp của mình.

### Azure AD license

- **Azure Active Directory miễn phí**: Cung cấp tính năng quản lý người dùng và nhóm, đồng bộ hóa thư mục tại chỗ, báo cáo cơ bản, thay đổi mật khẩu tự phục vụ cho người dùng đám mây và đăng nhập một lần trên Azure, Microsoft 365 và nhiều ứng dụng SaaS phổ biến.
- **Azure Active Directory Premium P1**: P1 cho phép người dùng kết hợp của bạn truy cập cả tài nguyên tại chỗ và đám mây. Hỗ trợ quản trị nâng cao, chẳng hạn như nhóm động, quản lý nhóm tự phục vụ, Microsoft Identity Manager và khả năng ghi lại trên đám mây, cho phép đặt lại mật khẩu tự phục vụ cho người dùng tại chỗ của bạn.
- **Azure Active Directory Premium P2**: cung cấp Bảo vệ danh tính Azure Active Directory để giúp cung cấp Quyền truy cập có điều kiện dựa trên rủi ro vào các ứng dụng của bạn và dữ liệu quan trọng của công ty và Quản lý danh tính đặc quyền để giúp khám phá, hạn chế và giám sát quản trị viên cũng như quyền truy cập của họ vào tài nguyên và cung cấp quyền truy cập đúng lúc khi cần thiết.
- **"Pay as you go" feature licenses**: Bạn cũng có thể nhận các giấy phép tính năng bổ sung, chẳng hạn như **Azure Active Directory Business-to-Customer (B2C)**. B2C có thể giúp bạn cung cấp các giải pháp quản lý danh tính và quyền truy cập cho các ứng dụng hướng tới khách hàng của bạn. 

### Các bước khởi tạo Azure AD 

1. Đăng nhập vào [Azure Portal](https://portal.azure.com) 

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/0001-createazuread.png)

2. Chọn **Create a resource**

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/0002-createazuread.png)

3. Trong trang **Create a resource**, bắt đầu tìm kiếm **Azure Active Directory** 

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/0003-createazuread.png)

4. Giao diện xuất hiện, chọn **Create**

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/0004-createazuread.png)

5. Trong trang **Create a tenant**

- Phần **Tenant type**, chọn **Azure Active Directory**

6. Chọn **Next:Configuration** 

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/0005-createazuread.png)

7. Trong **Configure your new directory**
   
- **Organization name**, Nhập tên **Azure AD** (Lưu ý tên phải duy nhất). Ví dụ: ```Firstcloudjourney```
- **Initial domain name**, nhập ```firstcloudjourney```

8. Chọn **Next: Review + create**

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/0006-createazuread.png)

9. Kiểm tra lại và chọn **Create**

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/0007-createazuread.png)

10. Bạn có thể bị hỏi nhập captcha để xác thực

- Nhập captcha
- Chọn **Submit**

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/0008-createazuread.png)

11. Sau đó chờ ít phút bạn sẽ có **Azure AD**.

12. Các bạn chọn vào tên tenant của bạn để xem thông tin.

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/0009-createazuread.png)


13. Nếu bạn thấy kết quả tương tự có nghĩa là bạn đã hoàn thành bước này. Chúng ta qua bước tiếp theo là tạo một số users trên Azure AD để sau này dùng user đó đăng nhập vào AWS.

![Create Azure AD](/images/2-Prerequiste/2.2-createAzureAD/00010-createazuread.png)
