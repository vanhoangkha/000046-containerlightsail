+++
title = "Push container image của bạn"
date = 2021
weight = 5
chapter = false
pre = "<b>4.5 </b>"
+++

Trong bước này, chúng ta sẽ tiến hành push container image lên Lightsail store để chuẩn bị triển khai cho dịch vụ Lightsail container của bạn.


1. Chạy câu lệnh sau để tiến hành push container image của chúng ta lên Lightsail store.
```
sudo aws lightsail push-container-image --service-name lightsail-container --label nginx-container-hello --image nginx-container
```
Sau khi push thành công, kết quả Lightsail sẽ trả về như dưới đây.
```
Image "nginx-container" registered.
Refer to this image as ":lightsail-container.nginx-container.hello.1" in deployments.
```
![Lightsail](/images/3/00025.png?featherlight=false&width=90pc)
{{%notice tip%}}
Nếu bạn chạy câu lệnh nhiều lần , push 1 image nhiều lần thì số đằng sau tên image sẽ tăng số thứ tự lên theo số lần bạn thực hiện push.
{{%/notice%}}

2. Vào giao diện quản trị [Lightsail container](https://lightsail.aws.amazon.com/ls/webapp/ap-southeast-1/container-services/lightsail-container/images)
  + Click tab **Images**.
  + Ở đây bạn có thể xem được các container image bạn đã push lên.

![Lightsail](/images/3/00026.png?featherlight=false&width=90pc)

3. Bước tiếp theo chúng ta sẽ thực hiện deploy mới sử dụng container image bạn vừa push lên.
