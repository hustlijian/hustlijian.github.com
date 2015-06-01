---
layout: post
title: "VPN 客户端配置全解"
categories: Tutorial
tags : [vpn, tutorial, client]
summary: VPN是上网必须呀，这里介绍了不同平台下VPN客户端的配置方法包括linux,mac, windows, android, ios。
---

VPN是上网必须呀，这里介绍了不同平台下VPN客户端的配置方法包括linux,mac, windows, android, ios。

转自：[云梯](https://www.yunti.me/guides/)

- [windows 7](#windows-7)
- [windows xp](#windows-xp)
- [windows 8](#windows-8)
- [mac osx](#mac)
- [linux/ubuntu](#ubuntu)
- [iPhone](#ios)
- [iPad](#ipad)
- [Android](#andriod)
- [智能加速](#chnroutes)

---

## windows 7

### 1.控制面板
点击电脑屏幕左下角的 Windows 标志，再点击“控制面板”，进入控制面板的设置
![image](/assets/img/vpn_client/step1-win7.jpg)

### 2.网络和 Internet

点击“网络和 Internet”文字，进入网络和 Internet的设置

![image](/assets/img/vpn_client/step2-win7.jpg)

### 3.网络和共享中心

点击“网络和共享中心”文字，进入网络和共享中心的设置

![image](/assets/img/vpn_client/step3-win7.jpg)

### 4.设置新的连接或网络

点击“设置新的连接或网络”文字

![image](/assets/img/vpn_client/step4-win7.jpg)

### 5.连接到工作区

选择“连接到工作区”，然后点击“下一步”按钮

![image](/assets/img/vpn_client/step5-win7.jpg)

### 6.使用我的 Internet 连接(VPN)

点击“使用我的 Internet 连接(VPN)”文字

![image](/assets/img/vpn_client/step6-win7.jpg)

### 7.Internet 地址，目标名称

“Internet 地址”中填入服务器域名（前往服务器列表页面查看）；“目标名称”中填入“云梯 VPN (PPTP)”；然后点击“下一步”按钮

![image](/assets/img/vpn_client/step7-win7.jpg)

### 8.用户名和密码

“用户名”中填入你的VPN帐号用户名；“密码”中填入你的VPN帐号密码；然后点击”连接“按钮

![image](/assets/img/vpn_client/step8-win7.jpg)

### 9.连接中

连接中

![image](/assets/img/vpn_client/step9-win7.jpg)

### 10.连接成功

连接成功

![image](/assets/img/vpn_client/step10-win7.jpg)

### 11.快速连接，断开

点击电脑屏幕右下角的网络标志，看到“云梯 VPN (PPTP)”的连接状态，通过“断开”或“连接”按钮，方便快速断开或连接 VPN

![image](/assets/img/vpn_client/step11-win7.jpg)

### 12.打开本地连接属性

在“控制面板 -> 网络和 Internet -> 网络和共享中心 -> 更改适配器设置”中找到“本地连接”，右键点击，然后点击“属性”；点击"Internet 协议版本4（TCP/IPv4）"，点击“属性”按钮

![image](/assets/img/vpn_client/step12-win7.jpg)

### 13.设置 DNS，防止 DNS 污染

选中“使用下面的 DNS 服务器地址”，“首选 DNS 服务器”中填写 8.8.8.8，“备用 DNS 服务器”中填写 8.8.4.4，然后点击“确定”按钮

![image](/assets/img/vpn_client/step13-win7.jpg)

### 14.清除 DNS 缓存

在“开始 -> 所有程序 -> 附件”中找到并打开“命令提示符”，输入以下命令并回车：ipconfig /flushdns

![image](/assets/img/vpn_client/step14-win7.jpg)

---

## windows xp
### 1.控制面板

点击电脑屏幕左下角的“开始”，再点击“控制面板”，进入控制面板的设置

![image](/assets/img/vpn_client/step1-xp.jpg)

### 2.网络和 Internet 连接

点击“网络和 Internet 连接”文字，进入网络和 Internet 连接的设置

![image](/assets/img/vpn_client/step2-xp.jpg)

### 3.创建到您的工作位置的网络连接

点击“创建⼀个到您的工作位置的网络连接”文字

![image](/assets/img/vpn_client/step3-xp.jpg)

### 4.虚拟专用网络连接

选择“虚拟专用网络连接”，点击“下一步”按钮

![image](/assets/img/vpn_client/step4-xp.jpg)

### 5.公司名

“公司名”中填入“云梯 VPN (PPTP)”；然后点击“下一步”按钮

![image](/assets/img/vpn_client/step5-xp.jpg)

### 6.主机名或 IP 地址

“主机名或 IP 地址”中填入服务器域名（前往服务器列表页面查看）；然后点击“下一步”按钮

![image](/assets/img/vpn_client/step6-xp.jpg)

### 7.添加快捷方式，完成

勾选“在我的桌面上添加一个到此连接的快捷方式”，然后点击“完成”按钮

![image](/assets/img/vpn_client/step7-xp.jpg)

### 8.网络连接

回到“网络和 Internet 连接”，点击“网络连接”文字

![image](/assets/img/vpn_client/step8-xp.jpg)

### 9.双击连接

在“虚拟专用网络”里看到之前新建的“云梯 VPN (PPTP)”，双击图标，打开连接窗口

![image](/assets/img/vpn_client/step9-xp.jpg)

### 10.用户名和密码

“用户名”中填入你的VPN帐号用户名；“密码”中填入你的VPN帐号密码；然后点击”连接“按钮

![image](/assets/img/vpn_client/step10-xp.jpg)

### 11.连接中

连接中

![image](/assets/img/vpn_client/step11-xp.jpg)

### 12.快速连接，断开

右键点击 VPN 桌面快捷方式，看到“云梯 VPN (PPTP)”的连接状态，通过“断开”或“连接”按钮，方便快速断开或连接 VPN

![image](/assets/img/vpn_client/step12-xp.jpg)

### 13.打开本地连接属性

在“控制面板 -> 网络和 Internet 连接 -> 网络连接”中找到“本地连接”，右键点击，然后点击“属性”；点击"Internet 协议（TCP/IP）"，点击“属性”按钮

![image](/assets/img/vpn_client/step13-xp.jpg)

### 14.设置 DNS，防止 DNS 污染

选中“使用下面的 DNS 服务器地址”，“首选 DNS 服务器”中填写 8.8.8.8，“备用 DNS 服务器”中填写 8.8.4.4，然后点击“确定”按钮

![image](/assets/img/vpn_client/step14-xp.jpg)

### 15.清除 DNS 缓存

在“开始 -> 所有程序 -> 附件”中找到并打开“命令提示符”，输入以下命令并回车：ipconfig /flushdns

![image](/assets/img/vpn_client/step15-xp.jpg)

---

## windows 8

### 1.控制面板

右键点击桌面左下角的 Windows 图标，再点击“控制面板”，进入控制面板的设置

![image](/assets/img/vpn_client/step1-win8.jpg)

### 2.网络和 Internet

点击“网络和 Internet”文字，进入网络和 Internet的设置

![image](/assets/img/vpn_client/step2-win8.jpg)

### 3.网络和共享中心

点击“网络和共享中心”文字，进入网络和共享中心的设置

![image](/assets/img/vpn_client/step3-win8.jpg)

### 4.设置新的连接或网络

点击“设置新的连接或网络”文字

![image](/assets/img/vpn_client/step4-win8.jpg)

### 5.连接到工作区

选择“连接到工作区”，然后点击“下一步”按钮

![image](/assets/img/vpn_client/step5-win8.jpg)

### 6.使用我的 Internet 连接(VPN)

点击“使用我的 Internet 连接(VPN)”文字

![image](/assets/img/vpn_client/step6-win8.jpg)

### 7.Internet 地址，目标名称

“Internet 地址”中填入服务器域名（前往服务器列表页面查看）；“目标名称”中填入“云梯 VPN (PPTP)”；然后点击“创建”按钮

![image](/assets/img/vpn_client/step7-win8.jpg)

### 8.连接

点击 Charm 栏中刚创建的“云梯 VPN (PPTP)”，然后点击“连接”按钮

![image](/assets/img/vpn_client/step8-win8.jpg)

### 9.用户名和密码

“用户名”中填入你的VPN帐号用户名；“密码”中填入你的VPN帐号密码；然后点击“确定”按钮，连接 VPN

![image](/assets/img/vpn_client/step9-win8.jpg)

### 10.连接成功

连接成功

![image](/assets/img/vpn_client/step10-win8.jpg)

### 11.快速连接和断开

点击桌面右下角的网络图标，可以在 Charm 栏中找到所有 VPN 配置，方便快速连接和断开 VPN

![image](/assets/img/vpn_client/step11-win8.jpg)

### 12.打开本地连接属性

在“控制面板 -> 网络和 Internet -> 网络和共享中心 -> 更改适配器设置”中找到本地连接（Wi-Fi 或者 Ethernet），右键点击，然后点击“属性”；点击"Internet 协议版本4（TCP/IPv4）"，点击“属性”按钮

![image](/assets/img/vpn_client/step12-win8.jpg)

### 13.设置 DNS，防止 DNS 污染

选中“使用下面的 DNS 服务器地址”，“首选 DNS 服务器”中填写 8.8.8.8，“备用 DNS 服务器”中填写 8.8.4.4，然后点击“确定”按钮

![image](/assets/img/vpn_client/step13-win8.jpg)

### 14.清除 DNS 缓存

右键点击桌面左下角的 Windows 图标，点击并打开“命令提示符”，输入以下命令并回车：ipconfig /flushdns

![image](/assets/img/vpn_client/step14-win8.jpg)

---

## mac

### 1.系统偏好设置

点击电脑屏幕左上角的苹果标志，在下拉选项里点击“系统偏好设置...”，进入系统的设置

![image](/assets/img/vpn_client/step1-mac.jpg)

### 2.网络

点击“网络”图标，进入网络的设置

![image](/assets/img/vpn_client/step2-mac.jpg)

### 3.添加 VPN 服务

点击左下方的“＋”号，添加 VPN 服务

![image](/assets/img/vpn_client/step3-mac.jpg)

### 4.接口，VPN 类型，服务名称

“接口”栏中选择“ VPN ”，选择后，下面的选项随之变化；“VPN 类型”栏中选择“ PPTP ”；”服务名称“中填入”云梯 VPN (PPTP)“；最后点击”创建“按钮

![image](/assets/img/vpn_client/step4-mac.jpg)

### 5.服务器地址，帐户名称

”服务器地址“中填入服务器域名（前往服务器列表页面查看）；”帐户名称“中填入你的VPN帐号用户名；最后点击”鉴定设置...“按钮

![image](/assets/img/vpn_client/step5-mac.jpg)

### 6.密码

”密码“中填入你的VPN帐号密码，然后点击”好“按钮

![image](/assets/img/vpn_client/step6-mac.jpg)

### 7.高级

点击”高级...“按钮，对 VPN 的使用方式进行设置

![image](/assets/img/vpn_client/step7-mac.jpg)

### 8.通过 VPN 连接发送所有流量

选中”通过 VPN 连接发送所有流量“，然后点击”好“按钮

![image](/assets/img/vpn_client/step8-mac.jpg)

### 9.连接

点击“连接”按钮，连接 VPN

![image](/assets/img/vpn_client/step9-mac.jpg)

### 10.连接成功

连接成功后的状态；建议勾选”在菜单栏中显示 VPN 状态“，可以在顶部菜单栏中显示连接情况，方便快速连接或断开 VPN

![image](/assets/img/vpn_client/step10-mac.jpg)

### 11.设置 DNS，防止 DNS 污染

在网络设置中，选中你的本地网络，如 Wi-Fi；点击“高级...”按钮，在 DNS 菜单下，添加 8.8.8.8 和 8.8.4.4 到 DNS 服务器中，最后点击“好”按钮

![image](/assets/img/vpn_client/step11-mac.jpg)

### 12.清除 DNS 缓存

打开 Terminal，根据你的系统版本运行对应的命令：

    dscacheutil -flushcache sudo discoveryutil udnsflushcaches

    Mac OS X 10.7 & 10.8 & 10.9
    sudo killall -HUP mDNSResponder

    Mac OS X 10.5 & 10.6
    dscacheutil -flushcache

    Mac OS X 10.4
    lookupd -flushcache

---

## ubuntu

### 1. 配置 VPN

点击屏幕左上角 Network Connections 标志，在下拉选项里点击 "VPN Connections"，点击 "Configure VPN..." 进入 VPN 的设置

![image](/assets/img/vpn_client/step1-ubuntu.jpg)

### 2.添加 VPN

点击 "VPN" 菜单下右侧的 "Add" 按钮，添加 VPN 服务

![image](/assets/img/vpn_client/step2-ubuntu.jpg)

### 3.选择 VPN 类型

选择 "Point-to-Point Tunneling Protocol (PPTP)"，点击 "Create..." 按钮

![image](/assets/img/vpn_client/step3-ubuntu.jpg)

### 4.填写 VPN 帐号信息

"Connection name"栏中填入“云梯 VPN (PPTP)”；"Gateway"中填入服务器域名（前往服务器列表页面查看）；"User name"中填入你的VPN帐号用户名；"Password"中填入你的VPN帐号密码；最后点击"Advanced..."按钮

![image](/assets/img/vpn_client/step4-ubuntu.jpg)

### 5.PPTP 高级选项

选中 "Use Point-to-Point encryption (MPPE)"，点击 "OK" 按钮

![image](/assets/img/vpn_client/step5-ubuntu.jpg)

### 6.保存 VPN

点击 "Save..." 按钮

![image](/assets/img/vpn_client/step6-ubuntu.jpg)

### 7.连接 VPN

点击 "VPN Connections" 下的“云梯 VPN (PPTP)”，开始连接 VPN

![image](/assets/img/vpn_client/step7-ubuntu.jpg)

### 8.连接成功

VPN 连接成功后系统会有提示信息，同时 Network Connections 上会有小锁的标志

![image](/assets/img/vpn_client/step8-ubuntu.jpg)

---

## ios

### 1.设置，通用

点击“设置”，进入系统的设置，点击“通用”

![image](/assets/img/vpn_client/step1-ios.jpg)

### 2.VPN

点击“ VPN ”，进入 VPN 设置

![image](/assets/img/vpn_client/step2-ios.jpg)

### 3.添加 VPN 配置

点击“添加 VPN 配置... ”，进入 VPN 配置

![image](/assets/img/vpn_client/step3-ios.jpg)

### 4.VPN 配置信息

协议类型选择“ PPTP ”；“描述”栏中填入“云梯 VPN (PPTP)”；“服务器”栏中填入服务器域名（前往服务器列表页面查看）；“帐户”栏中填入你的VPN用户名；“密码”栏中填入填入你的VPN密码；然后点右上角的"存储"按钮

![image](/assets/img/vpn_client/step4-ios.jpg)

### 5.连接

VPN 配置中会看到刚设置的"云梯 VPN (PPTP)"，选中后打开上方的 VPN 连接，状态改变为已连接

![image](/assets/img/vpn_client/step5-ios.jpg)

### 6.快速连接

VPN 配置成功后，在系统设置中会看到 VPN 的连接，可以快速连接或断开 VPN

![image](/assets/img/vpn_client/step6-ios.jpg)

---

## ipad

###1.设置，通用，VPN

点击桌面上的“设置”图标，进入系统的设置；点击左侧设置中的“通用”，再点击右侧的“ VPN ”，进入 VPN 设置

![image](/assets/img/vpn_client/step1-ipad.jpg)

### 2.添加 VPN 配置

点击右侧 VPN 中的“添加 VPN 配置... ”，进入 VPN 配置

![image](/assets/img/vpn_client/step2-ipad.jpg)

### 3.VPN 配置信息

协议类型选择“ PPTP ”；“描述”栏中填入“云梯 VPN (PPTP)”；“服务器”栏中填入服务器域名（前往服务器列表页面查看）；“帐户”栏中填入你的VPN用户名；“密码”栏中填入你的VPN密码；然后点右上角的"存储"按钮

![image](/assets/img/vpn_client/step3-ipad.jpg)

### 4.连接

VPN 配置中会看到刚设置的"云梯 VPN (PPTP)"，选中后打开上方的 VPN 连接，状态改变为已连接；VPN 配置成功后，在左侧设置中会看到 VPN 的连接，可以快速连接或断开 VPN

![image](/assets/img/vpn_client/step4-ipad.jpg)

---

## andriod

###1.设置，无线和网络

进入系统设置，点击“无线和网络”底部的“更多...”

![image](/assets/img/vpn_client/step1-android.jpg)

### 2.VPN

点击"VPN"，设置和管理 VPN

![image](/assets/img/vpn_client/step2-android.jpg)

### 3.添加 PPTP VPN

点击顶部"+"，“名称”栏中填入"云梯 VPN (PPTP)"；“类型”选择"PPTP"；“服务器地址”栏中填入服务器域名（前往服务器列表页面查看）；勾选“PPP 加密(MPPE)”；点击“保存”按钮

![image](/assets/img/vpn_client/step3-android.jpg)

### 4.设置成功

VPN 列表中会看到刚设置的 "云梯 VPN (PPTP)"，点击登录

![image](/assets/img/vpn_client/step4-android.jpg)

### 5.连接

"用户名"栏中填入你的VPN帐号用户名，"密码"栏中填入你的VPN帐号密码，然后点击“连接”按钮

![image](/assets/img/vpn_client/step5-android.jpg)

### 6.连接成功

连接成功后，VPN 列表中会显示“已连接”

![image](/assets/img/vpn_client/step6-android.jpg)

## chnroutes

[chnroutes](https://github.com/jimmyxu/chnroutes)

利用来自APNIC的数据生成路由命令脚本，让VPN客户端在连接时自动执行。通过这些路由脚本，可以让用户在使用VPN作为默认网关时，不使用VPN访问中国国内IP，从而减轻VPN负担，并提高访问国内网站的速度。

### Mac OS X

在终端中执行python chnroutes.py -p mac，这将生成ip-up和ip-down两个文件；

将这两个文件移入/etc/ppp/；

重新连接VPN，观察测试。

### Linux

执行python chnroutes.py -p linux，这将生成ip-pre-up和ip-down两个文件；

将ip-pre-up移入/etc/ppp/，ip-down移入/etc/ppp/ip-down.d/；

重新连接VPN，观察测试。

### Windows

在命令提示符中执行python chnroutes.py -p win，这将生成vpnup.bat和vpndown.bat两个文件；

在拨号前手动执行vpnup.bat文件设置路由表；在断开VPN后，可运行vpndown.bat清理路由表。

