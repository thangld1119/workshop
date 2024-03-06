---
title : "Thiết lập Application Loadbalance"
date :  "`r Sys.Date()`" 
weight : 8
chapter : false
pre : " <b> 8. </b> "
---


 Application Load Balancer là một dịch vụ phân phối tải trong AWS, được sử dụng để cân bằng tải lưu lượng đến các ứng dụng hoạt động trên nhiều máy chủ hoặc các tài nguyên xử lý ứng dụng khác nhau. Nó giúp tăng khả năng chịu tải, cải thiện hiệu suất và đảm bảo tính sẵn sàng của ứng dụng.

Bước đầu ta tạo *target group* cho loadbalance

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305155559.png)

Chọn VPC đã tạo

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305155652.png)

Ở đây mình sử dụng target group cho Web Host mở cổng 80 để bên ngoài Internet có thể truy cập vào trang web

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305155803.png)

Tạo Security Group cho Load Balance

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305160134.png)

Tạo Load Balance

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305160251.png)

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305160325.png)

Chú ý chọn 2 subnet public tại 2 zone

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305160445.png)

Security group

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305160626.png)

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305161025.png)

Sau khi xong chúng ta coppy DNS và tiến hành truy cập trang web thử

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305161202.png)

Thành quả

![](../images/8-SetUpApplicationLoadbalance/Pastedimage20240305161247.png)
