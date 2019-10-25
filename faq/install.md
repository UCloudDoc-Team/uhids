

# 安装报错

## 安装Agent提示“Permission denied”错误

您在 Linux 系统服务器中安装 Agent 时，收到“Permission denied”的错误提示。

您可以参考以下方法进行排查，并解决该问题。

1\. 检查是否通过 root 账号进行安装，并且执行`ls -al /etc/init.d/aegis`命令查看对于''
/etc/init.d/aegis'' 目录是否有执行权限。

2\. 查看您的服务器是否安装了云锁。您可以通过执行`ps -ef | grep yunsuo_agent`或'' ps aux | grep
yunsuo''命令进行检查。

如果服务器上已安装了云锁，可能会拦截Agent的安装。建议您暂时关闭云锁后，再尝试安装。

云锁的默认目录是 /usr/local/yunsuo\_agent。
