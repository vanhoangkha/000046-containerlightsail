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
![Lightsail](/images/3/00018.png?featherlight=false&width=90pc)

2. Chạy lệnh dưới đây để thêm Repo Docker.
```
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

![Lightsail](/images/3/00019.png?featherlight=false&width=90pc)

3. Tiến hành cài đặt Docker từ Repo bằng cách chạy câu lệnh dưới đây
```
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io -y
```

![Lightsail](/images/3/00020.png?featherlight=false&width=90pc)
 
4. Kiểm tra cài đặt Docker bằng câu lệnh dưới.
```
sudo docker run hello-world
```

![Lightsail](/images/3/00021.png?featherlight=false&width=90pc)

5. Bước tiếp theo chúng ta sẽ tiến hành build container image để tiến hành deploy.


![Lightsail](/images/3/00022.png?featherlight=false&width=90pc)