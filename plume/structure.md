## 目录结构
- bin 命令行工具
- config 配置文件
- docs 文档
- modules 应用代码
	1. 目录结构:example/Controller/IndexController.php
	2. example:模块名
	3. example/View:页面目录
	4. example/Controller：业务模块控制层
	5. example/Dao:数据访问层
	6. example/Service:业务逻辑层
	7. example/Utils:工具类
- templates 模板页面目录
- tests 测试代码
- var 数据目录
	1. var/cache:缓存
	2. var/logs:系统和业务日志
	3. var/sql:应用数据库脚本
- vendor 组件依赖目录
- web 应用发布目录

## 结构补充说明
- web/css css目录，建议使用common包含公共js文件，其他目录包含业务js文件
- web/js js目录，建议同css目录。
- web/images 图片存放目录，其他类型资源也建议如此。
- example/View/index 对应控制器视图目录
- example/View/layout 对应模块布局文件
- templates/errors 公共错误提示页面目录
- tests/Example/Tests 对应模块测试代码目录

## 文件补充说明
- 配置文件 env.php
- 入口文件 index_env.php
- 页面模板 layoutP.phtml用户PC,layoutM.phtml用于mobile
- 组件配置 composer.json

注:env是plume自定义环境变量