

# Agent安装和修复说明

Agent由用户决定是否安装

## 1、安装Agent

**支持的操作系统：**

  - CentOS
  - Ubuntu
  - Debian
  - RedHat
  - Open Suse
  - Gentoo

**安装命令：**

控制台中点击【安装命令】获取安装命令

![](/images/quick/安装命令.png)

在弹窗中复制安装命令后到linux操作系统中粘贴并执行。

![](/images/quick/安装脚本.png)

**检查是否安装成功：**

命令执行完查看agent是否正常启动：

`ps uax|grep uca`

能够检索到uca字样的文件即为成功。

![](/images/operation/图片1.png)

## 2、修复说明

如果发现Agent离线，无法传输数据，界面上不再显示告警提示信息。请重新安装一遍Agent，或者联系技术支持寻求帮助。
