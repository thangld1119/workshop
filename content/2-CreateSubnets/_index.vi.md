---
title : "Tạo subnet"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2. </b> "
---

Kế đến ta tạo 4 mạng con từ VPC mà chúng ta đã tạo trước đó
Trở lại *VPC console* và tạo *subnet*

![](../images/2-CreateSubnets/Pastedimage20240305115506.png)

Chú ý chọn VPC ID đúng với VPC vừa tạo

![](../images/2-CreateSubnets/Pastedimage20240305115656.png)

Tạo các subnet như bảng

| Subnet name        | IPv4 subnet   | Availability Zone |
| ------------------ | ------------- | ----------------- |
| workshop-pubsub-1  | 172.20.1.0/24 | us-west-1a        |
| workshop-pubsub-2  | 172.20.2.0/24 | us-west-1b        |
| workshop-privsub-1 | 172.20.3.0/24 | us-west-1a        |
| workshop-privsub-2 | 172.20.4.0/24 | us-west-1b        |

![](../images/2-CreateSubnets/Pastedimage20240305120736.png)

Làm tương tụ với các subnet còn lại

![](../images/2-CreateSubnets/Pastedimage20240305120828.png)

![](../images/2-CreateSubnets/Pastedimage20240305120917.png)

![](../images/2-CreateSubnets/Pastedimage20240305120957.png)

Sau khi thiết lập các *subnet* xong chúng ta tiến hành tạo. Và đây là thành quả

![](../images/2-CreateSubnets/Pastedimage20240305121159.png)

Sau khi tạo xong chúng ta mở tính năng *Auto-assign public IPv4 address* cho 2 public subnet
Tính năng *Auto-assign public IPv4 address* mỗi khi bạn triển khai một EC2 instance trong subnet thì sẽ được tự động được gán một địa chỉ IPv4 công cộng cho instance đó

![](../images/2-CreateSubnets/Pastedimage20240305123203.png)

![](../images/2-CreateSubnets/Pastedimage20240305123316.png)

![](../images/2-CreateSubnets/Pastedimage20240305123403.png)

