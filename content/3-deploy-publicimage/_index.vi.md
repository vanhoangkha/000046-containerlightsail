+++
title = "Triển khai public image"
date = 2021
weight = 3
chapter = false
pre = "<b>3. </b>"
+++


#### Triển khai container từ public image


1. Click **Deployments** tab.
  + Click **Create your first deployment**.

![Lightsail](/images/2/0001.png?featherlight=false&width=90pc)

2. Đặt caontainer name và image name **nginx**.
Soure container image có thể đến từ một kho lưu trữ công khai, như Docker Hub hoặc là những container image mà bạn đã tạo và lưu trữ bằng dịch vụ container image repo của mình.
Đối với bài lab này, chúng ta sẽ sử dụng container image docker Nginx chính thức do Nginx cung cấp. Docker Official Images là một tập hợp các kho lưu trữ Docker được tuyển chọn được lưu trữ trên Docker Hub đã được quét các lỗ hổng bảo mật và được duy trì bởi đội ngũ Docker.

![Lightsail](/images/2/0002.png?featherlight=false&width=90pc)

3. Bạn cũng có thể thêm các cấu hình tùy chọn như lệnh khởi chạy ban đầu, biến môi trường và các port mạng cho container. 
Đối với bài lab này, bạn không cần chỉ định lệnh khởi chạy hoặc các biến môi trường, nhưng cần mở port để kết nối tới nginx server.
Chúng ta sẽ cấu hình Container Nginx lắng nghe trên cổng 80 cho lưu lượng truy cập HTTP.
  + Click **Add open ports**.

![Lightsail](/images/2/0003.png?featherlight=false&width=90pc)

4. Điền thông tin port **80**. Protocol giữ nguyên **HTTP**.

![Lightsail](/images/2/0004.png?featherlight=false&width=90pc)

5. Để kiểm tra dịch vụ container đang hoạt động chính xác, chúng ta sẽ cần xác định public endpoint mà chúng ta có thể điều hướng đến trong trình duyệt web của mình.
Chúng ta sẽ chỉ định nginx làm container và đảm nhận các traffic tới public endpoint qua cổng 80. Đường dẫn health check (/) sẽ để giá trị mặc định.
  + Click **Save and deploy**.

![Lightsail](/images/2/0005.png?featherlight=false&width=90pc)


6. Sẽ mất vài phút để quá trình deploy container hoàn tất và trạng thái chuyển từ **Deploying** sang **Active**. 

![Lightsail](/images/2/0006.png?featherlight=false&width=90pc)

7. Kéo màn hình lên trên và click vào **public domain** của deployment để kết nối tới nginx container.

![Lightsail](/images/2/0007.png?featherlight=false&width=90pc)

8. Bạn sẽ kết nối tới server nginx đã được cài đặt trong container nginx của bạn. Bạn đã deploy container sử dụng public container image từ Docker Hub. Bước tiếp theo, chúng ta sẽ tự tạo container image và triển khai trên dịch vụ Lightsail container nhé.

![Lightsail](/images/2/0008.png?featherlight=false&width=90pc)