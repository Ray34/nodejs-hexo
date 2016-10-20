---
title: windows上安装mysql-5.7.16.zip
date: 2016-10-20 10:30:53
tags:
    - windows 
    - mysql
categories: 
    - 技术
---
### 注意事项

1、添加path环境变量；
2、修改my-default.ini文件里的port, basedir以及datadir并新建相应文件夹；
3、管理员权限运行cmd，进入mysql安装文件夹的bin目录下运行命令：

```bash
mysqld --initialize
mysqld -install/remove
net start mysql
mysql -u root -p
ALTER USER 'root'@'localhost' IDENTIFIED BY 'new_password'
```

初始化成功后在datadir目录下生成的文件中xxx.err里有root账户的临时密码：
2016-10-20T02:18:03.488650Z 1 [Note] A temporary password is generated for root@localhost: <font color=red>_i6Ry0xqIfwL</font>