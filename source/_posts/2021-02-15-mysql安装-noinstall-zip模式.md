---
title: mysql安装-no-install-zip模式
date: 2021-02-15 21:00:35
tags:
---

mysql安装-no-install-zip，使用zip格式文件安装mysql。
<!-- more -->
### mysql安装no-install-zip模式

> [mysql下载地址](https://dev.mysql.com/downloads/mysql/)
> [文档下载地址](https://dev.mysql.com/doc/refman/8.0/en/)

#### 1、提取zip
* 解压zip文件
#### 2、创建一个my.ini
* 创建一个自定义的配置文件，一个是安装文件，一个是数据文件
```
[mysqld]
# set basedir to your installation path
basedir=E:/mysql
# set datadir to the location of your data directory
datadir=E:/mydata/data
```
#### 3、初始化数据目录
* 安装目录\bin\mysqld --defaults-file=配置文件目录 --initialize --console  （随机生成密码）
  安装目录\bin\mysqld --defaults-file=配置文件目录 --initialize-insecure --console （不设置密码）
* 注意：配置文件中数据目录一定存在

#### 4、启动
* 安装目录\bin\mysqld --console
>  "C:\Program Files\MySQL\MySQL Server 8.0\bin\mysqld" --console
>   "C:\Program Files\MySQL\MySQL Server 8.0\bin\mysqladmin" -u root shutdown (关闭)

#### 5、客户端登录
* mysql -u root -p
* 安装时候没有设置密码：mysql -u root --skip-password
* 登录成功后修改密码：ALTER USER 'root'@'localhost' IDENTIFIED BY 'root-password';

> 创建账户：
> CREATE USER 'root'@'127.0.0.1' IDENTIFIED BY 'root-password';
  CREATE USER 'root'@'::1' IDENTIFIED BY 'root-password';

#### 6、设置环境变量和开机启动
* 设置环境变量MYSQL_HOME=D:\Program Files\mysql-8.0.23
> 设置完后，就可以执行全局执行mysql或者mysqld 

* 设置server作为service
>  "C:\Program Files\MySQL\MySQL Server 8.0\bin\mysqld" --install
>  sc start mysqld_service_name 
>  NET START mysqld_service_name
