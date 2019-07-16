# 实例管理

{{indexmenu_n>1}}

完成新建MySQL实例后，可以在控制台上管理MySQL实例，如：创建从库、配置升降级、数据库回档、备份管理、读写分离、重置密码、重启、日志管理、修改配置文件、更改实例名称、更改业务组、更改告警模板、删除、续费及监控告警等实例管理操作。

## MySQL基本操作

云数据库MySQL实例控制台基本操作主要有：启动、重启、关闭、重置密码、登录、更换配置文件、续费、删除等功能。

#### 启动MySQL实例

1.如果要启动处于关闭状态的MySQL实例，首先选择需要启动的MySQL实例，在列表右侧点击“启动”按钮，弹出的确认对话框选择确定，即可启动MySQL实例。

![image](/images/v4-001.png)

2.如果需要同时启动多个MySQL实例，选择相应的MySQL实例，在批量操作项中选择“启动”，弹出的对话框选择“确定”，即可启动多个MySQL实例。

![image](/images/v4-002.png)

#### 关闭MySQL实例

关闭单个MySQL实例，选择需要关闭实例，点击操作项中关闭按钮，弹窗确认关闭。

关闭实例会中断数据库服务，请谨慎操作。云数据库MySQL关闭功能提供强制关闭方式可以对MySQL实例进行强制关闭。

MySQL实例支持批量关闭多个实例，关闭操作步骤请参考启动MySQL实例。

#### 重启MySQL实例

MySQL实例支持单个重启和批量多个实例重启操作，具体操作步骤参考启动MySQL实例。

#### 删除MySQL实例

MySQL实例支持单个删除和批量删除，具体操作步骤参考启动MySQL实例。

#### 单个和批量MySQL实例操作

控制台支持单个和批量操作两种模式。

单个操作支持对选中的MySQL实例进行操作；批量操作支持对于多个MySQL实例进行共性的操作。

## 配置升降级

用户进行配置升降级操作可以选择不同数据库机型（标准机型和SSD机型）。

具体计费说明请参考“购买和计费”文档。

选中MySQL实例，在右侧下拉列表中选择配置升降级操作。

![image](/images/升降级01.png)

![image](/images/升降级02.png)

配置升降级开始后，MySQL实例状态显示为“升级中”，升级结束后，状态恢复为初始状态。

## 重置密码

选择需要修改密码的MySQL实例，点击操作项中“重置密码”按钮，弹窗中修改密码并确认。

![image](/images/mysqlpassword.png)

## 普通版升级高可用版

目前支持升级实例：实例处于运行中，该实例为普通版且没有从库。支持除北京A（无高可用版）、海外（无普通版）的所有机房。

操作步骤如下：

选定要升级的普通版实例，点击操作项中的“升级高可用”

![image](/images/image0.png)

升级高可用弹窗中选定高可用版，点击确认，完成支付差价，实例进入“数据同步中”

![image](/images/image1.png)

当实例完成数据同步，状态为“待切换高可用”时，点击操作项中“切换至高可用”确认切换

![image](/images/image2.png)

弹窗中确认切换

![image](/images/image3.png)

实例状态“切换中”当状态更新为“运行”时切换完成，实例升级到高可用版

![image](/images/image4.png)

### 操作日志

#### 查看操作日志

选中MySQL实例，在详情页选择操作日志。

![image](/images/操作日志.png)