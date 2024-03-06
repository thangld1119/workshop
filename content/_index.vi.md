---
title : "Thiết lập trang web với kiến trúc High Availability trên AWS"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
---

#### Giới thiệu về kiến trúc

Kiến trúc High Availability trên AWS.
Mục đích xây dựng kiến trúc này là đảm bảo tính sẵn sàng cao và khả năng phục hồi nhanh khi xảy ra sự cố cho hệ thống.

![](../images/Pastedimage20240306173225.png)

Kiến trúc được thiết kế gồm: 
- VPC được tạo tại 2 zone: us-west-1a và us-west-1b để tránh những sự cố xảy ra tại một zone đảm bảo tính sẵn sàng
- Có 2 public subnet và 2 private subnet đặt tại 2 zone
- Tạo 1 Internet Gateway và 2 Nat Gateway, 1 tại mỗi zone
- Sử dụng Aplication Loadbalance  để cân bằng tải cho trang web
- Sử dụng NACL, Security Groups và IAM cho bảo mật.
- Cấu hình Bastion host để quản trị từ internet
- 1 trang web trên Private subnet

#### Các bước tiến hành

1. [Tạo VPC](1-CreateVPC/)
2. [Tạo subnets](2-CreateSubnets/)
3. [Tạo Internet Gateway](3-CreateInternetGateway/)
4. [Thiết lập định tuyến](4-Routing/)
5. [Tạo Nat Gateway](5-CreateNatGateway/)
6. [Thiết lập Bastion Host](6-SettingBastionHost/)
7. [Thiết lập website trên EC2](7-SetUpWebsiteOnEC2/)
8. [Thiết lập Application Loadbalance](8-SetUpApplicationLoadbalance/)
9. [Kết thúc](9-End/)