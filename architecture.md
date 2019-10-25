

# 架构和原理简介

UHIDS(UCloud主机入侵检测系统)是UCloud安全中心推出的一款服务器安全产品。UHIDS主要由两个部分组成，即UHIDS-Server端和UHIDS-Agent端。通过在云主机上安装轻量级的Agent，并与云端UHIDS-Server端进行规则日志事件联动，实时监控云主机的安全性，保障云主机的安全。

![](/images/uhids架构.png)

UHIDS支持的服务器类型包括：

  - CentOS
  - Ubuntu
  - Debian
  - RedHat
  - Open Suse
  - Gentoo

通过加密传输服务器的相关数据到接口服务器上，由接口服务器再过滤风险数据和入侵数据分别到不同的集群中进行分析，分析的结果保存在数据库中。所有数据库中的数据整合到一个portal数据库供控制台页面进行调用。其中如果用户配置了需要告警提示，则告警的数据将实时通过邮件或者短信的方式发送给用户。
