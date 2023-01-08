+++
title = "Build container image của bạn"
date = 2021
weight = 4
chapter = false
pre = "<b>4.4 </b>"
+++

Trong bước này, chúng ta sẽ tiến hành build container image để triển khai cho dịch vụ Lightsail container của bạn.
Container image của chúng ta vẫn sử dụng image nginx nhưng thay thế file index.html để hiển thị lời chào.


1. Chạy câu lệnh sau để tạo thư mục chuẩn bị cho việc build image.Các câu lệnh tiếp theo sẽ chạy trong thư mục này.
```
mkdir lightsail-workshop-nginx
cd lightsail-workshop-nginx
```
![Lightsail](/images/3/00021.png?featherlight=false&width=90pc)

2. Chạy lệnh dưới đây để tạo file index.html
```
echo "Welcome to Amazon Lightsail Container workshop" > index.html
```

3. Chạy lệnh dưới đây để tạo Docker file.
```
echo "FROM nginx:latest" > Dockerfile
echo "COPY ./index.html /usr/share/nginx/html/index.html" >> Dockerfile
```
![Lightsail](/images/3/00022.png?featherlight=false&width=90pc)
4. Tiến hành build container image của chúng ta bằng cách chạy câu lệnh sau.
```
sudo docker build -t nginx-container .
```
![Lightsail](/images/3/00023.png?featherlight=false&width=90pc)

5. Chạy lệnh sau để chạy thử container image chúng ta vừa build trên Build Instance và kiểm tra kết quả.
```
sudo docker run -p 8080:80 nginx-container &
curl localhost:8080
```
![Lightsail](/images/3/00024.png?featherlight=false&width=90pc)

6. Bước tiếp theo chúng ta sẽ thực hiện push container image chúng ta vừa tạo lên Lightsail, để chuẩn bị thực hiện deploy.