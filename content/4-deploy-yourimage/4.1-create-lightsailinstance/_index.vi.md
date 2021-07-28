+++
title = "Tạo Lightsail instance"
date = 2021
weight = 1
chapter = false
pre = "<b>4.1 </b>"
+++

Trong bước này, chúng ta sẽ tạo Lightsail Instance.

1. Từ [giao diện quản trị của Lightsail](https://lightsail.aws.amazon.com/ls/webapp/home/) click **Create Instance**.


2. Click chọn nền tảng **Linux/Unix**. Dưới mục Blueprint, click chọn **OS Only*, sau đó chọn **Ubuntu Linux 20.04 LTS**.

![Lightsail](/images/container/013.png?width=90pc)

3. Kéo màn hình xuống dưới, ở mục **Identify your instance**, đặt tên instance của chúng ta là **Build-Instance**.

4. Kéo màn hình xuống dưới, click **Create Instance**.
![Lightsail](/images/container/014.png?width=90pc)

5. Chờ vài phút để Lightsail instance chuyển sang trạng thái running như bên dưới.
 + Click vào biểu tượng command line để kết nối tới Build-Instance.

![Lightsail](/images/container/015.png?width=90pc)

6. Cài đặt công cụ unzip cho Ubuntu
```
sudo apt-get install -y unzip
```
![Lightsail](/images/container/016.png?width=60pc)

7. Cài đặt AWS CLI trên Build-Instance bằng cách chạy các câu lệnh dưới đây
```
sudo curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
sudo unzip awscliv2.zip
sudo ./aws/install
```
![Lightsail](/images/container/017.png?width=60pc)

8. Cài đặt Lightsail control plugin cho AWS CLI bằng cách chạy các câu lệnh dưới đây
```
sudo curl "https://s3.us-west-2.amazonaws.com/lightsailctl/latest/linux-amd64/lightsailctl" -o "/usr/local/bin/lightsailctl"
sudo chmod +x /usr/local/bin/lightsailctl
```
![Lightsail](/images/container/018.png?width=60pc)

9. Bước tiếp theo chúng ta sẽ tạo user **awsstudent** có quyền **Administrator Access**, sau đó tạo accesskey / secret accesskey để cấu hình AWS CLI.