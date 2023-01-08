+++
title = "Thực hiện Deploy mới"
date = 2021
weight = 6
chapter = false
pre = "<b>4.6 </b>"
+++

Trong bước này, chúng ta sẽ tiến hành deploy container image lên Lightsail container service của bạn.


1. Truy cập vào [giao diện quản trị Lightsail container service của bạn](https://lightsail.aws.amazon.com/ls/webapp/ap-southeast-1/container-services/lightsail-container/deployments)
  + Click **Deployments**.
  + Click **Modify your deploy**

![Lightsail](/images/3/00028.png?featherlight=false&width=90pc)

2. Lựa chọn **":lightsail-container.nginx-container.hello.x"** container image.
![Lightsail](/images/3/00029.png?featherlight=false&width=90pc)

4. Kéo màn hình xuống dưới cùng và click **Save and Deploy** để tiến hành deploy.
![Lightsail](/images/3/00030.png?featherlight=false&width=90pc)

5. Bạn sẽ cần chờ vài phút để quá trình deploy hoàn tất.
  + Kéo màn hình lên trên và chờ trạng thái chuyển sang running.
  + Click vào Public domain để tiến hành truy cập tới dịch vụ đang chạy trong container của bạn. 
![Lightsail](/images/3/00031.png?featherlight=false&width=90pc)

6. Trang web mặc định của nginx đã được thay bằng dòng chữ **"Welcome to Amazon Lightsail Container workshop"**. Chúc mừng bạn đã hoàn tất bài lab Lightsail container.

7. Sau khi hoàn tất bạn hãy thực hiện dọn dẹp tài nguyên để tránh phát sinh chi phí ngoài mong muốn nhé.
