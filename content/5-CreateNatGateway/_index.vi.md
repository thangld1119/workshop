---
title : "Tạo Nat Gateway"
date :  "`r Sys.Date()`" 
weight : 5
chapter : false
pre : " <b> 5. </b> "
---

## Nat Gateway

Tiếp theo để có thể truy cập từ bên ngoài Cloud thì ta cần phải có địa chỉ IP chúng ta sẽ sử dụng dịch vụ *Elastic IP address* để có 1 địa chỉ ip

![](../images/5-CreateNatGateway/Pastedimage20240305130501.png)

![](../images/5-CreateNatGateway/Pastedimage20240305130345.png)

Tạo NAT gateway để các thành phần trong VPC giao tiếp với bên ngoài

![](../images/5-CreateNatGateway/Pastedimage20240305130530.png)

Chỉ cho phép public subnet giao tiếp ra môi trường internet

![](../images/5-CreateNatGateway/Pastedimage20240305130745.png)

