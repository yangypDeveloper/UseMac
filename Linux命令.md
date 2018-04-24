## 常用命令
> 平台 macOS

### telnet
我们都知道ping命令可以测试两个主机是否可以连接,eg:`ping 61.135.169.121`
如果我们想测试某个服务器的端口是否开启,就可以用`telnet`了,
下面是开启的情况

```
➜  ~ telnet 61.135.169.121 80
Trying 61.135.169.121...
Connected to 61.135.169.121.
Escape character is '^]'.
```
> 其实61.135.169.121 就是百度的一个ip服务器,可以用`w3m`命令,查看

```
Refresh (0 sec) /baidu.html?from=noscript
[bd_logo1][bd_logo1]
到百度首页到百度首页
[                    ][百度一下]
输入法

  • 手写
  • 拼音
  •
  • 关闭

百度首页设置登录
新闻hao123地图视频贴吧学术登录设置更多产品
网页新闻贴吧知道音乐图片视频地图文库更多»

百度

把百度设为主页关于百度About  Baidu百度推广

©2018 Baidu 使用百度前必读 意见反馈 京ICP证030173号  京公网安备11000002000001号
≪ ↑ ↓ Viewing <百度一下，你就知道>
```

### free
> 查看内存使用情况

```
[root@Li ~]# free
              total        used        free      shared  buff/cache   available
Mem:        1883492      389188      102036      490108     1392268      835364
Swap:        524284           0      524284
```


### Oracle服务启动和停止
启动

1. #su - oracle 切换到 oracle 用户且切换到它的环境
2. $lsnrctl status 查看监听及数据库状态
3. $lsnrctl start 启动监听
4. $sqlplus / as sysdba 以 DBA 身份进入 sqlplus
5. SQL>startup 启动 db

 停止
 
1. `#su - oracle #切换到 oracle 用户且切换到它的环境`
2. `$lsnrctl stop #停止监听`
3. `$sqlplus / as sysdba #以 DBA 身份进入 sqlplus`
4. `SQL>SHUTDOWN IMMEDIATE 关闭 db`


### 传送文件

scp 文件名 用户名@服务器ip:目标路径
```
scp /Users/yoli/Desktop/myerr.h root@192.168.31.86:/usr/include
```


