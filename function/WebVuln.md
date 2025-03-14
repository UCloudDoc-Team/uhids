

# Web漏洞检查

Web漏洞检查自动检测您服务器上的系统部署的Web服务和所使用的框架存在的风险点，并针对所发现的问题项为您提供修复建议。

## 检测原理

检测机制通过部署安装的客户端Agent在机器系统上查找对应的Web配置、Web环境设置以及指定参数等措施,利用加载的配置规则文件在本地上进行安全风险检测,不同的检测项采用不同的检测规则，检测是否符合一些风险特征,当命中风险规则后,从而提示风险点，及提供修复建议。

## 检测周期

- 每次插件启动或重新启动将立即扫描检测,其余默认定时每12个小时检测一次

- 清理风险后，12小时内会对该风险再次检测，如果发现风险已经修复，会自动删除该条告警。

## 检测项

| 分类  | 检测项            | 说明                               | 对应版本 |
| --- | -------------- | -------------------------------- | ---- |
| Web | Web-CMS 漏洞     | 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Wordpress SQL注入漏洞与提权漏洞（CVE-2015-2213）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Discuz 5.x 6.x 7.x 前台SQL注入漏洞| 最新的漏洞预警和相关补丁                    | V3.0 |
| Web | discuz7.2SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | tomcat管理后台| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | 未删除的.git目录| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | WordPressSQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | 未删除的.svn目录| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | phpMyAdmin登陆绕过登陆验证| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Thinkphp 3.0-3.1远程代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | finecms远程任意PHP代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | phpcmsv9.6.0版本SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | dedecms SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Joomla3.x SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | metinfo 5.3.1 注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | EmpireCMS sql注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | seacms 远程代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | FineCMS文件上传漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | FineCMS SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | beescms SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | SquirrelMail  远程代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | HDWiki SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Destoon 通用SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Drupal Core 8.4.x 远程代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Drupal Core 8.5.x 远程代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Drupal Core 7.x 远程代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | phpmailer远程代码执行| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Zabbix SQL注入漏洞(CVE-2013-5743)| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Cacti 任意命令执行漏洞(CVE-2014-2709)| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Yii SQL注入漏洞（CNNVD-201803-755）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | CodeIgniter远程PHP代码注入漏洞（CVE-2014-8684）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | phpinfo泄露| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | phpcms 9.3.1版本文件上传漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Discuz x3.2前台GET型SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Struts2-057 2.5.x版本存在远程代码执行漏洞CVE-2018-11776）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Struts2-057 2.3.x版本存在远程代码执行漏洞（CVE-2018-11776）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | jeecms V2.4.2 ArtiSearch.do 远程命令执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | 网站安装文件未删除| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | ECSHOP 2.7.3 代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | ECSHOP 3.x 代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | ECSHOP 2.7.2 SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Thinkphp 5.0.x-5.0.23 代码执行漏洞。| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | FastAdmin 远程代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | 未删除的.ds_store文件| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | 未删除的.idea目录| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Drupal SA-CORE-2019-003远程命令执行| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Nexus Repository Manager3远程代码执行漏洞(CVE-2019-7238)| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Confluence未授权RCE(CVE-2019-3396)漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Jenkins反序列化远程代码执行漏洞（CVE-2015-8103）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Jenkins反序列化远程代码执行漏洞（CVE-2017-1000353）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Piwik超级用户插件上传漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Piwik远程代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Piwik 2.16.0 对象注入| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Struts2-048远程代码执行漏洞（CVE-2017-9791）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Struts2-053远程代码执行漏洞（CVE-2017-12611）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Wordpress任意文件上传漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | PHPMailer 远程代码执行漏洞（CVE-2016-10033）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Jenkins 远程代码执行漏洞（CVE-2019-1003000）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | phpmyadmin 任意文件包含/远程代码执行漏洞（CVE-2018-19968）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | WebLogic Server反序列化漏洞(CVE-2019-2725)| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | 数据库文件泄露| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Jenkins反序列化远程代码执行漏洞（CVE-2015-8103）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Thinkphp 3.2.3版本存在SQL注入漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | phpunit 远程代码执行漏洞（CVE-2017-9841）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Drupal任意文件上传漏洞（CVE-2020-13671）| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Joomla远程代码执行漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Confluence未授权RCE(CVE-2021-26048)漏洞| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Cacti 远程代码执行漏洞(CVE-2024-25641)| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |
| Web | Cacti 远程代码执行漏洞(CVE-2024-29895)| 请跟进最新的漏洞预警和相关补丁                    | V3.0 |


<wrap em>对应版本指产品的版本号，可以参见升级记录查看版本号及对应升级内容。</wrap>
