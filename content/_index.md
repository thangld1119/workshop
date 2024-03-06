---
title : "Setting up a High Availability website architecture on AWS"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
---

#### Introduction to architecture

High Availability Architecture on AWS.
The purpose of building this architecture is to ensure high availability and fast recoverability when incidents occur for the system.

![](../images/Pastedimage20240306173225.png)

The architecture is designed as follows:
- A VPC is created across 2 zones: us-west-1a and us-west-1b to avoid outages caused by incidents in a single zone and ensure high availability.
- There are 2 public subnets and 2 private subnets placed across the 2 zones.
- 1 Internet Gateway and 2 Nat Gateways are created, with 1 in each zone.
- An Application Load Balancer is used to balance load for the website.
- NACLs, Security Groups and IAM are used for security.
- A Bastion host is configured for remote administration from the internet.
- 1 website is deployed on the Private subnet.

#### Steps to take

1. [Create VPC](1-CreateVPC/)
2. [Create Subnets](2-CreateSubnets/)
3. [Create Internet Gateway](3-CreateInternetGateway/)
4. [Routing](4-Routing/)
5. [Create Nat Gateway](5-CreateNatGateway/)
6. [Setting Bastion Host](6-SettingBastionHost/)
7. [Set Up Website On EC2](7-SetUpWebsiteOnEC2/)
8. [Set Up Application Loadbalance](8-SetUpApplicationLoadbalance/)
9. [End](9-End/)