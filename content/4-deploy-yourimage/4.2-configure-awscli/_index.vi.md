+++
title = "Cấu hình AWS CLI"
date = 2021
weight = 2
chapter = false
pre = "<b>4.2 </b>"
+++

Trong bước này, chúng ta sẽ tạo IAM user access key và secret access key để sử dụng cấu hình cho AWS CLI.

1. Từ [giao diện của dịch vụ IAM](https://console.aws.amazon.com/iam/home#/home) click **Users**.
![Lightsail](/images/container/019.png?width=90pc)

2. Click **Add users*

![Lightsail](/images/container/020.png?width=90pc)

3. Đặt tên user là **aws-cli**.
  + Click chọn **Programmatic access**, user của chúng ta chỉ sử dụng cho AWS CLI nên không cần đăng nhập vào management console.
  + Click **Next: Permissions**.

![Lightsail](/images/container/021.png?width=90pc)

4. Click **Attach existing policies directly**.
  + Click chọn **Administrator Access**.
  + Click **Next: Tags**.

![Lightsail](/images/container/022.png?width=90pc)

5. Click **Next: Review**. sau đó click **Create User**.

6. Click **Download .csv** để download file csv chứa thông tin access và secret access key.
![Lightsail](/images/container/023.png?width=90pc)

7. Quay lại Build Instance của chúng ta chạy lệnh **sudo aws configure** để tiến hành cấu hình CLI.
  + Cấu hình thông tin Region và format như hình dưới. Lưu ý sử dụng access key và secret access key từ file csv bạn download về.
![Lightsail](/images/container/024.png?width=60pc)

8. Bước tiếp theo chúng ta sẽ cài đặt Docker để bắt đầu thực hiện build image.