---
title : "Kết nối đến máy chủ Public"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 3.1. </b> "
---
![SSMPublicinstance](/images/arc-02.png)

1. Truy cập vào [giao diện quản trị của dịch vụ EC2](https://console.aws.amazon.com/ec2/v2/home).
  + Click chọn **Tích vào ô gitlab-runner**.
  + Click **Connect**.

![Connect](/images/3.connect/31.png)

1. Sau khi connect xong.
  + Sử dụng lệnh **sudo -i** để tiến vào user root.

2. Truy cập vào [project mà bạn đã push lên truớc dó ](https://gitlab.com/)
  + Tiếp đến ta chọn **Settings**
  + Click **CICD**.
![Connect](/images/3.connect/32.png)
  + Click **Expand Runner**.
![Connect](/images/3.connect/33.png)


1. Sau đó chọn **New project runner** 
![Connect](/images/3.connect/34.png)

2. Tiếp đến ở mục **tags**
  + Setname mục **tags** mà bạn muốn
  + Mục **Configuration (optional)** đặt tên như bên trên bạn đặt
  + Tích chọn **Create Runner**

![Connect](/images/3.connect/35.png)


1. Sau khi create runner xong tích chọn **Linux** 
2. Kéo xuống dưới ta sẽ thấy dòng chữ **How do iintall Gitlab Runner?**
  + Tích chọn vào đấy . Tích chọn xong ta sẽ thấy như bên ảnh , rồi sau đó ta copy hết vào chuyển sang **console AWS**
![Connect](/images/3.connect/37.png)
  + Paste hết thứ ta vừa copy vào và Enter
3. Sau khi paste xong ta trở về gitlab runner copy như trong ảnh
![Connect](/images/3.connect/38.png)
  + Rồi quay trở lại **console AWS** dán vào
![Connect](/images/3.connect/39.png)
Sử dụng lệnh **vi /etc/gitlab-runner/config.toml** đê chỉnh số lương gitlab runner có thể chạy trên các project . Ở đây mình chỉnh là 4
![Connect](/images/3.connect/30.png)


