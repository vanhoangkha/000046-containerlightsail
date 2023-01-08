+++
title = "Cấu hình AWS CLI"
date = 2021
weight = 2
chapter = false
pre = "<b>4.2 </b>"
+++

Trong bước này, chúng ta sẽ tạo IAM user access key và secret access key để sử dụng cấu hình cho AWS CLI.

1. Từ [giao diện của dịch vụ IAM](https://console.aws.amazon.com/iam/home#/home) click **Users**.

![Lightsail](/images/3/00010.png?featherlight=false&width=90pc)

1. Click **Add users*

![Lightsail](/images/3/00011.png?featherlight=false&width=90pc)

2. Đặt tên user là **aws-cli**.
  + Click chọn **Programmatic access**, user của chúng ta chỉ sử dụng cho AWS CLI nên không cần đăng nhập vào management console.
  + Click **Next: Permissions**.

![Lightsail](/images/3/00012.png?featherlight=false&width=90pc)

3. Click **Attach existing policies directly**.
  + Click chọn **Administrator Access**.
  + Click **Next: Tags**.

![Lightsail](/images/3/00013.png?featherlight=false&width=90pc)

4. Click **Next: Review**. sau đó click **Create User**.

5. Click **Download .csv** để download file csv chứa thông tin access và secret access key.

![Lightsail](/images/3/00014.png?featherlight=false&width=90pc)

6. Quay lại Build Instance của chúng ta chạy lệnh **sudo aws configure** để tiến hành cấu hình CLI.
  + Cấu hình thông tin Region và format như hình dưới. Lưu ý sử dụng access key và secret access key từ file csv bạn download về.

![Lightsail](/images/3/00015.png?featherlight=false&width=90pc)

7. Bước tiếp theo chúng ta sẽ cài đặt Docker để bắt đầu thực hiện build image.

![Lightsail](/images/3/00016.png?featherlight=false&width=90pc)
