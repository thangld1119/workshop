---
title : "Setting Bastion Host"
date :  "`r Sys.Date()`" 
weight : 6
chapter : false
pre : " <b> 6. </b> "
---


Bastion Host is limiting and controlling external access to servers in a private network. Instead of allowing direct external access to the servers, users must first connect to Bastion Host through a secure channel where they use SSH and then from Bastion Host, they can access other servers in the private network

First we will create a Security Group to set rules for Bastion Host
Go to the EC2 console and proceed to create a Security Group

![](../images/6-SettingBastionHost/Pastedimage20240305143949.png)

![](../images/6-SettingBastionHost/Pastedimage20240305143010.png)

SSH unlock 

![](../images/6-SettingBastionHost/Pastedimage20240305143649.png)

Create a KeyPair for Bastion Host

![](../images/6-SettingBastionHost/Pastedimage20240305144119.png)

![](../images/6-SettingBastionHost/Pastedimage20240305144408.png)

Save keypair

![](../images/6-SettingBastionHost/Pastedimage20240305144447.png)

Create EC2 as a Bastion Host server

![](../images/6-SettingBastionHost/Pastedimage20240305144659.png)

Here I use Ubuntu

![](../images/6-SettingBastionHost/Pastedimage20240305144838.png)

Select the newly created keypair

![](../images/6-SettingBastionHost/Pastedimage20240305144928.png)

VPC security group parameters

![](../images/6-SettingBastionHost/Pastedimage20240305145122.png)

And proceed to run Instances

![](../images/6-SettingBastionHost/Pastedimage20240305151239.png)

Proceed with SSH access to the Bastion server
Here I use git bash to access the corresponding command and the downloaded keypair file above

![](../images/6-SettingBastionHost/Pastedimage20240305151411.png)

![](../images/6-SettingBastionHost/Pastedimage20240305151741.png)

The Bastion Host has been set up
