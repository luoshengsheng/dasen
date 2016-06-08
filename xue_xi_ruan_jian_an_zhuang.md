# 学习软件安装

## mysql安装

### A、编译安装
          [博客地址](http://www.cnblogs.com/xiongpq/p/3384681.html)
### B、yum，rpm安装

### C、遇到问题记录
      1.提示：mysql command not found
          执行命令的时候，系统在/usr/bin下面查此命令，找不到
          解决办法：ln -s /usr/local/mysql/bin/mysql /usr/bin
      2.外网访问mysql
          要给地址授权才能在外网登录，下面是给所有的外网地址授权，然后刷新权限（在mysql命令框下执行）
          grant all privileges on *.* to root@'%' identified by 'QUSTDJX'
          flush privileges;