---
title : "Create Nat Gateway"
date :  "`r Sys.Date()`" 
weight : 5
chapter : false
pre : " <b> 5. </b> "
---


Next, to be able to access from outside the Cloud, we need to have an IP address, we will use the service *Elastic IP address* to have 1 ip address

![](../images/5-CreateNatGateway/Pastedimage20240305130501.png)

![](../images/5-CreateNatGateway/Pastedimage20240305130345.png)

Create a NAT gateway for components in the VPC to communicate with the outside

![](../images/5-CreateNatGateway/Pastedimage20240305130530.png)

Only allow public subnets to communicate to the internet environment

![](../images/5-CreateNatGateway/Pastedimage20240305130745.png)

