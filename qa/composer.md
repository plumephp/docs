
## 常见composer命令

- 刷新autoload
```
composer dump-autoload
```
- 更新相同版本的plume
```
composer clearcache
composer update plume/plume
```
- 更新不同版本的plume
```
composer update plume/plume
```
- 指定全局composer国内镜像
```
composer config -g repo.packagist composer https://packagist.phpcomposer.com
```
注：镜像站会有同步时间差
- 不安装dev依赖
```
composer inatall --no-dev --optimize-autoloader
```