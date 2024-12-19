

# 安全基线检查

安全基线检查自动检测您服务器上的系统、中间件、数据库、账号配置存在的风险点，并针对所发现的问题项为您提供修复建议。

## 检测原理

检测机制通过部署安装的客户端Agent在机器系统上查找对应的应用配置、环境设置以及指定参数等措施,利用加载的配置规则文件在本地上进行安全风险检测,不同的检测项采用不同的检测规则，检测是否符合一些风险特征,当命中风险规则后,从而提示风险点，及提供修复建议。

## 检测周期

- 每次插件启动或重新启动将立即扫描检测,其余默认定时每12个小时检测一次

- 清理风险后，12小时内会对该风险再次检测，如果发现风险已经修复，会自动删除该条告警。

## 检测项

| 分类  | 检测项            | 说明                               | 对应版本 |
| --- | -------------- | -------------------------------- | ---- |
| 系统  | 是否存在账号弱口令      | 检查Linux系统登录账号的密码是否是弱口令           | V3.0 |
| 系统  | 是否存在非root特权账号  | 检查Linux系统的是否存在非root用户但有root权限的账号 | V3.0 |
| 应用  | 是否使用不安全SSH协议版本 | 检查是否使用了不安全的安全协议                  | V3.0 |
| 应用  | 是否允许SSH空口令登录   | 检查SSH是否允许空口令登录                   | V3.0 |
| 应用  | Nginx是否高权限运行检测 | 检查Nginx是否以root权限运行               | V3.0 |
| 应用  | Apache是否高权限运行  | 检查Apache Httpd是否以root权限运行        | V3.0 |
| 应用  | 是否存在PHP版本信息泄露  | 检查是否存在PHP配置不当导致版本信息泄露            | V3.0 |
| 应用  | 是否存在PHP可执行高危函数 | 检查PHP配置中是否禁用可执行高危函数              | V3.0 |
| 应用  | 是否存在Java环境漏洞 | 检查Java环境变量与配置中是否存在风险（例如:apache-log4j 漏洞）              | V3.0 |
| 数据库 | MySQL是否高权限运行   | 检查MySQL服务是否以root权限运行             | V3.0 |
| 数据库 | Mongodb是否启用验证  | 检查Mongodb配置中是否开启密码验证             | V3.0 |
| 中间件 |	Redis未设置密码验证 |  检查redis服务的配置是否开启密码验证
| 数据库 |	Mongodb未启用验证   |   检查服务于配置的设置情况,避免默认启用有风险的选项 | V3.0 |
| 数据库 |	Mongodb监听地址存风险 |   非必要请勿将MongoDB监听地址设置在全地址监听状态,避免公网暴露情况 | V3.0 |
| 应用   |	Tomcat未禁用账号    |   修改Tomcat配置,非必要请去除或禁用账号后台登陆情况 | V3.0 |
| 应用   |	Tomcat高权限运行    |   修改Tomcat运行的进程权限,避免使用高权限运行该服务 | V3.0 |
| 应用   |	Tomcat未删除样例包  |   请删除在Tomcat Web目录下的样例包,避免更多的敏感信息泄露 | V3.0 |
| 应用   |	Tomcat允许目录浏览  |   请关闭Tomcat目录浏览功能,避免信息泄露 | V3.0 |
| 应用   |	Tomcat未禁止自动部署|   非必要请避免开启自动部署,避免遭到黑客入侵攻击 | V3.0 |
| 应用   |	Tomcat未禁用JMX远程 |   非必要请避免开启JMX远程部署,避免遭到黑客入侵攻击 | V3.0 |
| 应用   |	Caddy高权限运行      |   修改Caddy运行的进程权限,避免使用高权限运行该服务 | V3.0 |
| 应用   |	Hadoop未开启访问验证  |   检查服务于配置的设置情况,避免默认启用有风险的选项 | V3.0 |
| 应用   |	Apache开启重写配置    |   检查服务于配置的设置情况,避免默认启用有风险的选项 | V3.0 |
| 应用   |	Hadoop ResourceManager 公网暴露 |   非必要请勿将Hadoop 后台接口服务监听地址设置在全地址监听状态,避免公网暴露情况 | V3.0 |
| 应用   |	Nginx错误配置导致目录遍历 |   检查服务于配置的设置情况,避免默认启用有风险的选项 | V3.0 |
| 应用   |	Nginx错误配置导致目录穿越 |   检查服务于配置的设置情况,避免默认启用有风险的选项 | V3.0 |
| 应用   |	Nginx错误配置导致CRLF注入 |   检查服务于配置的设置情况,避免默认启用有风险的选项 | V3.0 |


<wrap em>对应版本指产品的版本号，可以参见升级记录查看版本号及对应升级内容。</wrap>