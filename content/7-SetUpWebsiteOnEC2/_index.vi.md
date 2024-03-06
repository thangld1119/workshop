---
title : "Thiết lập website trên EC2"
date :  "`r Sys.Date()`" 
weight : 7
chapter : false
pre : " <b> 7. </b> "
---


# Thiết lập trang web trên EC2
Tiến hành tạo thêm 1 EC2 tại private subnet
Đầu tiền tạo keypair cho host website

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305152059.png)

Lưu nó ở thư mục keypair của Bastion Host 

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305152420.png)

Tiến hành gửi keypair cho Bastion Host

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305152838.png)

Tiếp đến tạo Instances Web

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305153529.png)

Thiết lập Security Group cho Instance Web chỉ có thể truy cập từ Bastion Host

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305153814.png)

Tiếp theo ta sử dụng Bastion Host truy cập vào Máy chủ Web

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305154211.png)

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305154340.png)

Cài các thư viện cần thiết

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305154506.png)

Kiếm tài nguyên web ở đây mình tải tại trang tooplate 

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305154956.png)

Tiến hành giải nén và coppy vào thư mục html và restart lại dịch vụ httpd

![](../images/7-SetUpWebsiteOnEC2/Pastedimage20240305155424.png)

