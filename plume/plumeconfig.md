## 框架配置文件
```
web/index_dev.php
web/index_test.php
web/index_pro.php
```
## 定制框架
```
// 指定根路径
$app['plume.root.path'] = __DIR__.'/../';
// 指定默认模块
$app['plume.module.default']='example';
// 开启请求缓存
$app['plume.cache.request']=true;
// 设置缓存过期时间
$app['plume.cache.request.expires']=20;
// 设置缓存详细路由和过期时间
$app['plume.cache.config']=array(
	'/example/index/index' => 5,
	'/example/index/edit' => 2,
	'/example/index/save' => 0,
);
// 开启数据库缓存
$app['plume.cache.db']=true;
// 定制默认模板页面
$app['plume.templates.300']= 'templates/errors/index.html';
$app['plume.templates.404']= 'templates/errors/404.html';
$app['plume.templates.500']= 'templates/errors/500.html';
```