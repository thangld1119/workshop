---
title : "Thiết lập Bastion Host"
date :  "`r Sys.Date()`" 
weight : 6
chapter : false
pre : " <b> 6. </b> "
---


## Thiết lập Bastion Host

Bastion Host là giới hạn và kiểm soát quyền truy cập từ bên ngoài vào các máy chủ trong mạng riêng. Thay vì cho phép truy cập trực tiếp từ bên ngoài vào các máy chủ, người dùng trước tiên phải kết nối đến Bastion Host thông qua một kênh bảo mật ở đây mình sử dụng SSH và sau đó từ Bastion Host, họ có thể truy cập các máy chủ khác trong mạng riêng

Đầu tiên chúng ta sẽ tạo Security Group để thiết lập quy tắc cho Bastion Host
Vào EC2 console và tiến hành tạo Security Group

![](../images/6-SettingBastionHost/Pastedimage20240305143949.png)

![](../images/6-SettingBastionHost/Pastedimage20240305143010.png)

Mở khóa SSH 

![](../images/6-SettingBastionHost/Pastedimage20240305143649.png)

Tiến hành tạo KeyPair cho Bastion Host

![](../images/6-SettingBastionHost/Pastedimage20240305144119.png)

![](../images/6-SettingBastionHost/Pastedimage20240305144408.png)

Lưu keypair

![](../images/6-SettingBastionHost/Pastedimage20240305144447.png)

Tiến hành tạo EC2 để làm máy chủ Bastion Host

![](../images/6-SettingBastionHost/Pastedimage20240305144659.png)

Ở đây mình sử dụng Ubuntu

![](../images/6-SettingBastionHost/Pastedimage20240305144838.png)

Chọn keypair vừa mới tạo

![](../images/6-SettingBastionHost/Pastedimage20240305144928.png)

Thông số VPC , security group

![](../images/6-SettingBastionHost/Pastedimage20240305145122.png)

Và tiến hành chạy Instances

![](../images/6-SettingBastionHost/Pastedimage20240305151239.png)

Tiến hành truy cập SSH vào máy chủ Bastion
Ở đây mình sử dụng git bash để truy cập theo lệnh tương ứng và tệp keypair đã tải xuống ở trên

![](../images/6-SettingBastionHost/Pastedimage20240305151411.png)

![](../images/6-SettingBastionHost/Pastedimage20240305151741.png)

Như vậy đã thiết lập xong Bastion Host
