## 使用git安装
- 创建plume项目
```
git clone https://github.com/zhangbaitong/plume-skeleton.git proName
```
- 安装依赖
```
cd proName
composer install
```
如果安装依赖时间比较长，建议再次更新依赖，也可以指定全局的composer镜像
```
composer config -g repo.packagist composer https://packagist.phpcomposer.com
```
- 创建数据库
导入数据库脚本并启动数据库
```
proName/var/sql/init.sql
```
修改数据库配置文件
```
proName/config/dev.php
proName/config/test.php
proName/config/pro.php
```
- 运行单元测试
在proName目录打开命令行窗口
```
./vendor/bin/phpunit
```
- 启动服务
```
php -S 127.0.0.1:8081 -t web/ web/index_dev.php
```
- 查看示例
```
http://localhost:8081/
http://localhost:8081/example/index
```