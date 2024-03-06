---
title : "Create Subnets"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2. </b> "
---

Next, we will create 4 subnets under the VPC that was previously created.
Go back to the VPC console and create subnets.

![](../images/2-CreateSubnets/Pastedimage20240305115506.png)

Note that you should select the correct VPC ID that matches the VPC that was just created.

![](../images/2-CreateSubnets/Pastedimage20240305115656.png)

Create subnets such as tables

| Subnet name        | IPv4 subnet   | Availability Zone |
| ------------------ | ------------- | ----------------- |
| workshop-pubsub-1  | 172.20.1.0/24 | us-west-1a        |
| workshop-pubsub-2  | 172.20.2.0/24 | us-west-1b        |
| workshop-privsub-1 | 172.20.3.0/24 | us-west-1a        |
| workshop-privsub-2 | 172.20.4.0/24 | us-west-1b        |

![](../images/2-CreateSubnets/Pastedimage20240305120736.png)

Do the same with the rest of the subnets

![](../images/2-CreateSubnets/Pastedimage20240305120828.png)

![](../images/2-CreateSubnets/Pastedimage20240305120917.png)

![](../images/2-CreateSubnets/Pastedimage20240305120957.png)

After setting up the *subnet* we proceed to create. And here's the result.

![](../images/2-CreateSubnets/Pastedimage20240305121159.png)

After creating the subnets, enable the "Auto-assign public IPv4 address" feature for the two public subnets.
The "Auto-assign public IPv4 address" feature automatically assigns a public IPv4 address to EC2 instances when they are launched in that subnet.

![](../images/2-CreateSubnets/Pastedimage20240305123203.png)

![](../images/2-CreateSubnets/Pastedimage20240305123316.png)

![](../images/2-CreateSubnets/Pastedimage20240305123403.png)

