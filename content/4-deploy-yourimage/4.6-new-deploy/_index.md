+++
title = "Thực hiện Deploy mới"
date = 2021
weight = 6
chapter = false
pre = "<b>4.6 </b>"
+++

Trong bước này, chúng ta sẽ tiến hành deploy container image lên Lightsail container service của bạn.


1. Truy cập vào [giao diện quản trị Lightsail container service của bạn] (https://lightsail.aws.amazon.com/ls/webapp/ap-southeast-1/container-services/lightsail-container/deployments)
  + Click **Deployments**.
  + Click **Modify your deployment**.
![Lightsail](/images/container/032.png?width=90pc)

2. Click **Choose stored image** để tiến hành lựa chọn container image bạn đã push.
![Lightsail](/images/container/033.png?width=90pc)

3. Lựa chọn **":lightsail-container.nginx-container.hello.x"** container image.
![Lightsail](/images/container/034.png?width=90pc)

4. Kéo màn hình xuống dưới cùng và click **Save and Deploy** để tiến hành deploy.
![Lightsail](/images/container/035.png?width=90pc)

5. Bạn sẽ cần chờ vài phút để quá trình deploy hoàn tất.
  + Kéo màn hình lên trên và chờ trạng thái chuyển sang running.
  + Click vào Public domain để tiến hành truy cập tới dịch vụ đang chạy trong container của bạn. 
![Lightsail](/images/container/036.png?width=90pc)

6. Trang web mặc định của nginx đã được thay bằng dòng chữ **"Welcome to Amazonlightsail Container workshop"**. Chúc mừng bạn đã hoàn tất bài lab Lightsail container.
![Lightsail](/images/container/037.png?width=50pc)


7. Sau khi hoàn tất bạn hãy thực hiện dọn dẹp tài nguyên để tránh phát sinh chi phí ngoài mong muốn nhé.
