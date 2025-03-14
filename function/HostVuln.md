

# 主机漏洞检查

主机漏洞安全检查主要包含的是主机系统内的软件包管理工具提供下载安装的软件漏洞检查,包含系统大部分原生工具及组件与内核,均可以通过该检查项进行安全检测.

## 检测原理

这里采用读取软件包管理数据库的方式,获取当前系统已安装的软件信息,上传到云端与自建漏洞库进行漏洞匹配分析,分析产出的漏洞信息将提供给前台界面展示.

## 检测周期

- Agent插件启动后立即执行扫描
- 默认定时每12个小时检测一次
- 清理风险后，12小时内会对该风险再次检测，如果发现风险已经修复，会自动删除该条告警。

## 检测项

| 分类  | 检测项            | 说明                               | 对应版本 |
| --- | -------------- | -------------------------------- | ---- |
| rpm  | Redhat      | 支持检查Linux软件漏洞,包含Redhat系统类型软件漏洞检测           | V3.0 |
| rpm  | CentOS      | 支持检查Linux软件漏洞,包含CentOS系统类型软件漏洞检测           | V3.0 |
| rpm  | Rocky       | 支持检查Linux软件漏洞,包含Rocky系统类型软件漏洞检测            | V3.0 |
| deb  | Ubuntu      | 支持检查Linux软件漏洞,包含Ubuntu系统类型软件漏洞检测           | V3.0 |
| deb  | Debian      | 支持检查Linux软件漏洞,包含Debian系统类型软件漏洞检测           | V3.0 |


<wrap em>对应版本指产品的版本号，可以参见升级记录查看版本号及对应升级内容。</wrap>
