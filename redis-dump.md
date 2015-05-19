redis合并多个数据

>reids-dump工具

说一下安装，文档这里有 https://github.com/delano/redis-dump

apt-get install ruby

apt-get install ruby1.9.1-dev

gem install redis-dump

php环境下这3步不可少

使用示例：

导出`redis-dump -u 127.0.0.1:6379 > redis_data.json`

导入  `cat redis_data | redis-load -u 120.0.0.1:6379`
