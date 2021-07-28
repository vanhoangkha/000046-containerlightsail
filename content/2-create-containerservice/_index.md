+++
title = "Tạo container service"
date = 2021
weight = 2
chapter = false
pre = "<b>2. </b>"
+++


#### Tạo container service


1. Quay trở lại giao diện [Lightsail console](https://lightsail.aws.amazon.com/ls/webapp/home/). Click vào tab **Container**.
  + Click **Create container service**

![Lightsail](/images/container/001.png?width=90pc)

2. Chọn một vị trí cho dịch vụ container của bạn bằng cách chọn một AWS Region gần bạn hoặc gần khách hàng của bạn. Đối với lab này, chúng ta sẽ sử dụng Region Singapore.
  + Chọn mức cấu hình dịch vụ container mà bạn sẽ cần (bao gồm bộ nhớ và công suất xử lý). Cấu hình bạn chọn xác định sức mạnh tính toán, bộ nhớ và chi phí cho dịch vụ container của bạn.

![Lightsail](/images/container/002.png?width=90pc)

3. Kéo màn hình xuống dưới, đặt tên cho dịch vụ container của bạn  là **lightsail-container** sau đó click **Create container service**.

![Lightsail](/images/container/003.png?width=90pc)

4. Sẽ mất vài phút để quá trình tạo dịch vụ container hoàn tất và trạng thái chuyển sang Ready. Bước tiếp theo chúng ta sẽ thực hiện triển khai một deployment từ 1 container image lấy từ public repo ( kho lưu trữ công cộng).

![Lightsail](/images/container/004.png?width=90pc)