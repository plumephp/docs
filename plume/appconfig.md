## 应用配置文件
```
config/dev.php
config/test.php
config/pro.php
```
## 数据库配置
```
return array(
	'db' => array(
        'driver' => 'mysql',
        'host' => 'localhost',
        'username'=>'root',
        'password'=>'',
        'database'=>'plume',
        'port' => '3306',
        'charset'=>'utf8'
	),
);
```
## 自定义配置
```
return array(
	'db' => ...,
	'page' => array(
		'key1' => 'value1',
		'key2' => 'value2'
	),
);
```
