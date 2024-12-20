

# Agent管理

查看已安装和未安装Agent的主机信息。

![](/images/operation/agent管理.png)

表1.Agent列表参数

| 参数      | 说明                                                         |
| ------- | ---------------------------------------------------------- |
| 主机ID    | 主机的资源ID地址以及资源描述,常见于UCloud云主机,非UCloud云主机则无该字段内容    |
| 主机IP    | 主机的IP地址，默认显示内网IP以及公网IP,非UCloud云主机无法显示公网IP             |
| 可用区    | UCloud资源主机所在的可用区位置                                                 |
| 系统版本  | 显示已安装UHIDS主机入侵检测Agent插件的主机当前系统版本信息                      |
| Agent状态 | 共计2种状态：已安装和未安装。[安装agent参见此处](uhids/quick/agent)。 |
| 企业版有效期 | 展示的是已开通的企业版UHIDS的有效时间,超过有效期则表示企业版过期 |
| 最近上线时间 | 展示的是最近一段时间接收到UHIDS主机入侵检测Agent客户端上报的心跳时间,上报时间于当前时间相差大于2小时即表示插件异常失联状态需要排查问题 |
| 操作      | 点击【查看】后可跳转到uhost此主机所在的管理页面, 点击【切换版本】即可从基础版升级到企业版,或者由企业版转变到基础版                          |
