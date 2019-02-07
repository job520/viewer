> viewer
>> 自用日志查看器  
>> 官方文档：[点击进入](http://doc.job520.net/web/#/page/edit/3/42)

### 1. 引入：
1. 下载：  
`
composer require job520/viewer
`
2. 引入：  
`
require_once "vendor/autoload.php";
`
### 2. 用法：
1. 示例代码：
```
<?php
// 1. 引入包
require_once 'vendor/autoload.php';
// 2. 使用命名空间
use job520\viewer;
// 3. 定义要查看的目录
$base ='files/';
// 4. 定义请求路径，如：/log/index.php
$request_uri = $_SERVER['REQUEST_URI'];
// 5. 设置用户名/密码验证（可选）
$auth = array(
    'username' => 'user',
    'password' => 'pass'
);
// 6. 实例化对像
$obj = new viewer($base,$request_uri,$auth);
// 7. 运行
$obj->run();
```
2. 效果：
![](http://doc.job520.net/server/../Public/Uploads/2019-02-06/5c5b013bbdc1d.png)
![](http://doc.job520.net/server/../Public/Uploads/2019-02-02/5c55ad1815087.png)
