## 环境依赖

- 依赖版本
PHP版本 >= 5.5,windows使用plume-installer需要VS运行库。  
建议使用PHP7和64位系统。

- 提交plume-skeleton到自己的仓库
```
rm .git
```

- PHP安装版本下载
```
http://php.net/downloads.php
http://windows.php.net/download/
```
- windows下设置环境变量
```
我的电脑->属性->高级->环境变量->系统变量->Path->编辑
然后在"变量值"最前处加上"D:/php;D:/php/ext;"
```
- windows下composer不可以用
```
Your requirements could not be resolved to an installable set of package
composer selfupdate
Composer\Exception\NoSslException
composer config -g -- disable-tls true
Composer\Downloader\TransportException
修改php.ini
extension_dir = "F:\php7\ext"
extension=php_curl.dll
extension=php_gd2.dll
extension=php_mbstring.dll
extension=php_mysqli.dll
extension=php_openssl.d
extension=php_pdo_mysql.dll
```
