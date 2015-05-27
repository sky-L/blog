redis合并多个数据

>reids-dump工具

说一下安装，使用文档这里有 https://github.com/delano/redis-dump

>Ubuntu环境
```
apt-get install ruby

apt-get install ruby1.9.1-dev

gem install redis-dump

php环境下这3步不可少
```
>centos环境
```
yum install ruby rubygems ruby-devel   //安装rubygems 以及相关包  

gem sources -a http://ruby.taobao.org/   //加入淘宝，外面的源不能访问  

gem sources -r http://rubygems.org/     //删除默认的源
 
gem install redis-dump -V    //安装redis-dump
```
使用示例：

导出`redis-dump -u 127.0.0.1:6379 > redis_data`

导入  `cat redis_data | redis-load -u 120.0.0.1:6379`
