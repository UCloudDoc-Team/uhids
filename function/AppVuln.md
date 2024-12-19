

# 应用漏洞检查

应用漏洞检查自动检测您服务器上部署的常见应用风险点，并针对所发现的问题项为您提供修复建议。

## 检测原理

检测机制通过部署安装的客户端Agent在机器系统上查找应用的版本以及指定参数等措施,利用加载的配置规则文件在本地上进行安全风险检测,不同的检测项采用不同的检测规则，检测是否符合一些风险特征,当命中风险规则后,从而提示风险点，及提供修复建议。

## 检测周期

- 每次插件启动或重新启动将立即扫描检测,其余默认定时每12个小时检测一次

- 清理风险后，12小时内会对该风险再次检测，如果发现风险已经修复，会自动删除该条告警。

## 检测项

| 分类  | 检测项            | 说明                               | 对应版本 |
| 应用   |	Apache HTTPD 多后缀解析漏洞 |   检查服务于配置的设置情况,避免默认启用有风险的选项 | V3.0 |
| 应用   |	Apache Log4J2 RCE漏洞(CVE-2021-44228) |   请及时升级运行中的Apache Log4J版本 | V3.0 |
| 应用   |	Apache ActiveMQ 远程代码执行漏洞 |   请及时升级当前部署的Apache ActiveMQ版本 | V3.0 |
| Web应用|  Web-CMS 漏洞     | 最新的漏洞预警和相关补丁。                    | V3.0 |
| 应用   |	OpenSSH 远程代码执行漏洞 |   请及时升级当前部署的OpenSSH版本 | V3.0 |
| 应用   |	MySQL2远程代码执行漏洞 |   请及时升级当前部署的MySQL2版本 | V3.0 |
| 应用   |	Apache Kafka访问控制不当漏洞 |   请及时升级当前部署的Kafka版本 | V3.0 |
| 应用   |	liblzma/xz工具库恶意后门植入漏洞 |   请及时升级当前部署的xz版本 | V3.0 |
| 应用   |	runc容器逃逸漏洞 |   请及时升级当前部署的Docker版本 | V3.0 |
| 应用   |	OpenSSH ProxyCommand命令注入漏洞 |   请及时升级当前部署的OpenSSH版本 | V3.0 |
| 应用   |	Fortinet FortiOS SSL-VPN 远程代码执行漏洞 |   请及时升级当前部署的Fortinet FortiOS SSL-VPN版本 | V3.0 |
| 应用   |	泛微E-Office任意代码执行漏洞 |   请及时升级当前部署的泛微E-Office版本 | V3.0 |
| 应用   |	Jenkins Remoting 任意文件读取漏洞 |   请及时升级当前部署的Jenkins版本 | V3.0 |

<wrap em>对应版本指产品的版本号，可以参见升级记录查看版本号及对应升级内容。</wrap>