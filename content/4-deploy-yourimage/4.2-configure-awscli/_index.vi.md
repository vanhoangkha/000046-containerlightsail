---
title: "Hướng Dẫn Cấu Hình AWS CLI"
date: 2021-01-01
weight: 2
chapter: false
pre: "<b>4.2 </b>"
---

#### Bước Đầu Cấu Hình AWS CLI

Amazon Web Services (AWS) là một nền tảng cung cấp dịch vụ đám mây đa năng và mạnh mẽ. Để quản lý các dịch vụ AWS một cách nhanh chóng thông qua Command Line Interface (CLI), bạn cần thiết lập AWS CLI bằng cách tạo các access keys cho IAM User. Sau đây là hướng dẫn từng bước để bạn có thể thực hiện quá trình này một cách thuận lợi.

**Bước 1:** Đăng nhập vào AWS Management Console
- Truy cập AWS Management Console tại link: [https://console.aws.amazon.com/iam/](https://console.aws.amazon.com/iam/).

**Bước 2:** Chọn IAM User
- Tại IAM console, truy cập vào "Users" trong navigation pane và click vào tên người dùng mà bạn muốn tạo access key.

**Bước 3:** Tạo Access Key
- Trên trang thông tin người dùng, đi đến tab "Security credentials" và trong phần "Access keys", click "Create access key".

**Bước 4:** Thiết lập Access Key trong CLI
- Trong quá trình cấu hình, chọn "Command Line Interface (CLI)".

**Bước 5:** Nhập Tags (nếu cần)
- Bạn có thể nhập tags cho access key nếu muốn và sau đó click "Next".

**Bước 6:** Tải File .csv
- Click vào "Download .csv file" để tải về file chứa access key ID và secret access key.

**Bước 7:** Hoàn thành tạo key
- Sau khi file .csv đã được tải về, click "Done" để hoàn tất.

**Lưu ý quan trọng:** Access key là dữ liệu nhạy cảm và cần được bảo mật. Hãy lưu trữ file .csv cẩn thận và không chia sẻ cho những người không tin cậy.

Theo các bước trên, việc tạo và cấu hình AWS CLI trở nên đơn giản, giúp bạn quản lý tài nguyên AWS một cách linh hoạt qua CLI.

