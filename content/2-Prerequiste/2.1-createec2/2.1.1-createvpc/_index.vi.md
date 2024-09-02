---
title : "Tạo EC2 "
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 2.1.1 </b> "
---


#### Tạo EC2 **
1. Truy cập [giao diện quản trị dịch vụ EC2](https://console.aws.amazon.com/ec2/v2/home)
  + Click **Launch Instance**.

![EC2](/images/2.prerequisite/ec2.png)

1. Keo xuong 
  + Tại mục **Name tag** điền **gitlab-runner**.
![EC2](/images/2.prerequisite/1.2.png)
  + Click **Ubuntu**.
![EC2](/images/2.prerequisite/13.png)
  + Click **Create security group**.
  + Click **Allow SSH traffic from**.
  + Click **Allow HTTPS traffic from the internet**.
  + Click **Allow HTTP traffic from the internet**.

![EC2](/images/2.prerequisite/14.png)
