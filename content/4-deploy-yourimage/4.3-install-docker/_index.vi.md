+++
title = "Cài đặt Docker cho Ubuntu"
date = 2021
weight = 3
chapter = false
pre = "<b>4.3 </b>"
+++

Trong bước này, chúng ta sẽ tiền hành cài đặt Docker cho Lightsail Instance của chúng ta để thực hiện build container image.
Bạn có thể tham khảo thêm qui trình cài đặt [tại đây](https://docs.docker.com/engine/install/ubuntu/)

1. Chạy câu lệnh sau để cài đặt các gói cần thiết và thêm vào  GPG ( GNU Privacy Guard ) key để có thể sử dụng repository của Docker.
```
sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
![Lightsail](/images/container/025.png?width=60pc)

2. Chạy lệnh dưới đây để thêm Repo Docker.
```
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
![Lightsail](/images/container/026.png?width=60pc)

3. Tiến hành cài đặt Docker từ Repo bằng cách chạy câu lệnh dưới đây
```
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io -y
```
 
4. Kiểm tra cài đặt Docker bằng câu lệnh dưới.
```
sudo docker run hello-world
```
![Lightsail](/images/container/027.png?width=60pc)

5. Bước tiếp theo chúng ta sẽ tiến hành build container image để tiến hành deploy.