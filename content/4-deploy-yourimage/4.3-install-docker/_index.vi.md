+++
title = "Cài đặt Docker cho Ubuntu"
date = 2021
weight = 3
chapter = false
pre = "<b>4.3 </b>"
+++

Trong bước này, chúng ta sẽ tiền hành cài đặt Docker cho Lightsail Instance của chúng ta để thực hiện build container image.
Bạn có thể tham khảo thêm qui trình cài đặt [tại đây](https://docs.docker.com/engine/install/ubuntu/)


1. Cài đặt Docker

- Gói cài đặt Docker có sẵn trong kho lưu trữ chính thức của Ubuntu có thể không phải là phiên bản mới nhất. Để chắc chắn rằng chúng ta có được phiên bản mới nhất, chúng ta sẽ cài đặt Docker từ kho lưu trữ chính thức của Docker. Để làm điều này, chúng ta sẽ thêm một nguồn gói mới, thêm khóa GPG từ Docker để đảm bảo rằng các tải xuống là hợp lệ, sau đó cài đặt gói đó.

- Đầu tiên, cập nhật danh sách gói hiện có của bạn:

```
sudo apt update
```

2. Tiếp theo, cài đặt một số gói tiên quyết cho phép apt sử dụng gói qua HTTPS:

```
sudo apt install apt-transport-https ca-certificates curl software-properties-common
```

3. Sau đó thêm khóa GPG cho kho lưu trữ chính thức của Docker vào hệ thống của bạn:

```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```

4. Thêm kho lưu trữ Docker vào nguồn APT:

```
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
```

5. Điều này cũng sẽ cập nhật cơ sở dữ liệu gói của chúng ta với các gói Docker từ repo mới được thêm vào.

Đảm bảo rằng bạn sẽ cài đặt từ kho lưu trữ Docker thay vì kho lưu trữ Ubuntu mặc định:

```
apt-cache policy docker-ce
```

6. Bạn sẽ thấy đầu ra tương tự như sau, mặc dù số phiên bản của Docker có thể khác:

```
Output của apt-cache policy docker-ce
docker-ce:
  Installed: (none)
  Candidate: 5:19.03.9~3-0~ubuntu-focal
  Version table:
     5:19.03.9~3-0~ubuntu-focal 500
        500 https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
```

7. Lưu ý rằng docker-ce chưa được cài đặt, nhưng ứng viên cho việc cài đặt lại đến từ kho lưu trữ Docker cho Ubuntu 20.04 (focal).

Cuối cùng, cài đặt Docker:

```
sudo apt install docker-ce
```

8. Docker giờ đây đã được cài đặt, quá trình daemon đã được khởi động, và đã được thiết lập để tự động chạy khi hệ thống khởi động. Kiểm tra xem nó đã đang chạy chưa:

```
sudo systemctl status docker
```

 
9. Kiểm tra cài đặt Docker bằng câu lệnh dưới.
```
sudo docker run hello-world
```

![Lightsail](/images/3/00021.png?featherlight=false&width=90pc)

10. Bước tiếp theo chúng ta sẽ tiến hành build container image để tiến hành deploy.


![Lightsail](/images/3/00022.png?featherlight=false&width=90pc)