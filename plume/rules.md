## 路由匹配
请求地址
```
http://localhost:8080/example/index/list
```
Action处理类
```
modules/example/Controller/IndexController/listAction
```
视图
```
modules/example/View/index/list.phtml
```
## 视图数据
Action返回数据
```
//users为用户返回数据中的key
$data['users']
```
系统数据
```
//error为Action中设置error()函数显示指定的状态
$plume['error']
//Action切面前置方法返回数据
$plume['before']
//Action切面后置方法返回数据
$plume['after']
//项目根全路径
$plume['ROOT_PATH']
```





