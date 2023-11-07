---
title: "Chuẩn bị"
date: 2021
weight: 1
chapter: false
pre: "<b>1. </b>"
---

### Chuẩn bị

Trước khi bắt đầu với bài lab này, hãy đảm bảo rằng bạn đã nắm được các khái niệm cơ bản để chuẩn bị sẵn sàng cho bài lab.

**Giao diện dòng lệnh AWS (CLI)**  
Giao diện dòng lệnh AWS (CLI) là một công cụ hợp nhất giúp bạn quản lý các dịch vụ AWS qua dòng lệnh và trong các script. Trong bài lab này, bạn sẽ sử dụng AWS CLI để tương tác với các dịch vụ và triển khai vùng chứa Amazon Lightsail. Hãy cài đặt AWS CLI bằng cách làm theo các hướng dẫn sau:

- [Cài đặt AWS CLI](https://000011.awsstudygroup.com/vi/1-cli-installation/)
- [Thiết lập CLI cơ bản](https://000011.awsstudygroup.com/vi/2-basic-setup/)

**AWS Identity and Access Management (IAM)**  
IAM là một dịch vụ trong AWS giúp bạn kiểm soát truy cập vào tài nguyên AWS một cách an toàn. Bạn có thể sử dụng IAM để quản lý việc xác thực và ủy quyền khi sử dụng tài nguyên AWS.

- [Quản trị quyền truy cập với IAM](https://000002.awsstudygroup.com/vi/)

**Docker**  
Docker cung cấp nền tảng cho phép bạn phát triển và chạy ứng dụng trong môi trường container. Trong bài lab này, bạn sẽ sử dụng Docker để xây dựng và quản lý các container image, sau đó triển khai chúng trên Amazon Lightsail.


#### Tổng quan về Dịch vụ Container AWS Lightsail

AWS Lightsail cung cấp tài nguyên máy tính để triển khai hình ảnh Docker, sau đó được tự động chạy trên cơ sở hạ tầng của AWS.

Nguồn: [Dịch vụ container trong Amazon Lightsail](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-containers)

#### Tạo và Quản lý Các Bản Triển khai

Hướng dẫn cụ thể về cách tạo và quản lý các bản triển khai cho dịch vụ container Lightsail.

Nguồn: [Tạo và quản lý các bản triển khai cho dịch vụ container Amazon Lightsail](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-creating-and-managing-deployments)

#### Tạo Dịch vụ Container

Các bước chi tiết để tạo một dịch vụ container Lightsail, bao gồm việc chọn một khu vực AWS thông qua bảng điều khiển Lightsail.

Nguồn: [Tạo dịch vụ container Amazon Lightsail](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-creating-container-services)

#### Dung lượng Dịch vụ Container

Thông tin về việc chọn dung lượng cho một dịch vụ container, ảnh hưởng đến quy mô và sức mạnh của nó.

Nguồn: [Tạo một dịch vụ container Lightsail - Amazon Lightsail](https://docs.aws.amazon.com/lightsail/)


#### Quản lý Hình ảnh Container

Hướng dẫn về việc đẩy và quản lý hình ảnh container trong dịch vụ container Lightsail.

Nguồn: [Đẩy và quản lý hình ảnh container trên Amazon Lightsail](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-pushing-and-managing-container-images)

#### Tạo Hình ảnh Container

Các bước về cách tạo hình ảnh container cho Lightsail, bao gồm chạy một hình ảnh container mới và xây dựng một Dockerfile.

Nguồn: [Tạo hình ảnh container cho dịch vụ container Amazon Lightsail](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-creating-container-images)
