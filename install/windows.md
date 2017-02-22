## windows(64位)系统环境安装

- 下载安装工具
```
https://github.com/zhangbaitong/plume-installer/tree/master/dist/windows/plume-installer.exe
```
- 创建plume项目  
在plume-install当前目录打开命令行窗口
```
plume-installer new proName 1
```
如果安装依赖时间比较长，建议再次更新依赖
```
cd proName
composer install
```
也可以指定全局的composer镜像
```
composer config -g repo.packagist composer https://packagist.phpcomposer.com
```
- 创建数据库
导入数据库脚本并启动数据库
```
proName\var\sql\init.sql
```
修改数据库配置文件
```
proName\config\dev.php
proName\config\test.php
proName\config\pro.php
```
- 运行单元测试
在proName目录打开命令行窗口
```
.\vendor\bin\phpunit.bat
```
- 启动服务
```
.\start.bat
```
- 查看示例
```
http://localhost:8081/
http://localhost:8081/example/index
```