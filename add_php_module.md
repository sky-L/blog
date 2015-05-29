>php 打模块 

以mongo为例：centoos 	(源码编译)
	```	
	访问github网站然后搜索"mongo php driver"
	
	1  	/usr/local/php/bin/phpize

	2 	在模块下目录中  ./configure -h 查看所有编译参数会看到--with-php-config
		

		然后 ./configure --with-php-config=/usr/local/php/bin/php-config --enable-mongo

		make && make install

	3	编辑php.ini增加extension=mongo

	4 	重启http服务  /usr/local/apache2/bin/apachectl restart
	```

>ubuntu下就很方便 -- 

	```
	 apt-get install php5-redis (php5+模块名)
	```
