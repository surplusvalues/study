1、shutdown -S -t 60  一分钟后关机
2、Shutdown -a 取消关机计划
3、Shutdown -l 注销计算机
4、Tasklist 列出正在运行的进程
5、Command MMc启动计算机管理
6、chkdsk(检查磁盘,默认为C盘
7、taskmgr启动任务管理器
8、tsshutdn(60秒后关机）
9、rononce -p(15秒后关机)

**1 .ipconfig**
功能：查询本机ip信息
格式：ipconfig/XX
例：
(1）ipconfig/release：释放本机本机现有IP
(2）ipconfig/renew :向DHCP服务器重新申请一个Ip(可理解成你家的路由器）
(3)   ipconfig/all：显示完整版的ip

**2.nslookup**
功能: 查询网站ip地址
格式: nslookup 网站域名

**3.Ping**
功能：测试网络连通性
格式：ping域名/ip地址(参数)

**4.netstat**
功能：查询网络状态。看到网络的很多详细信息
例：
netstat -a：查看开启了哪些端口,常用netstat -an
netstat -n：查看端口的网络连接情况，常用netstat -an
netstat -v：查看正在进行的工作
netstat -p 协议名：
例：
netstat -p tcglip 查看某协议使用情况(查看tcplip协议使用情况)
netstat -s：查看正在使用的所有协议使用情况
**5.tracert**
功能：跟踪路由信息
查出数据从本地机器传输到目标主机经过所有的途径
这对我们了解网络布周和结构很有帮助
格式：tracert -参数ip(或计算机名）跟踪路由(数据包)
参数：“-w数字”用于设置超时间隔
例：
tracert www.baidu.com
**6.net**
功能：网络命令中最重要的，功能太强大。子命令很多
例如：net use、net start、net stop等。
例：
net start：查看开启了哪些服务
net start 服务名：开启服务
net stop 服务名：止某服务
net config：显示系统网络设置
net Logoff：断开连接的共享
net pause 服务名：暂停某服务
net send ip："文本信息"向对方发信息
net ver：局域网内正在使用的网络连接类型和信息
net share：查看本地开启的共享
net user 用户名密码：将用户登陆后将密码改为12345
net password密码：更改系统登陆密码

**7 .telnet**
功能：功能强大的远程登陆命令
史用自己的机器一样，只要你熟悉DOS命令
在成功以administrator身份连接了远程机器后
就可以用它来干你想于的一切
格式：telnet 远程机器地址
open ip：连接到IP（属telnet登陆后的命令）
**8.ftp**
功能：任何人都可以登陆上去
现在如果你扫到一归开放的ft服务主机
(一般都是开了21端口的机器），你想干唯干唯