# 空间管理

该功能主要是基于时间维度，统计数据库实例实际的物理空间(库/表磁盘) 和库表空间信息。
让用户能够掌握数据库实例的整体空间使用情况，对空间大小做合理的规划和管理，
同时能够帮助用户检索库/表的结构和使用情况，引导用户优化表设计。

## 进入空间管理

在“实例管理“页面的数据库列表"操作"栏中，点击“空间管理”，进入“空间管理”页面。

![image](/images/space-manage-010.png)
![image](/images/space-manage-020.png)

“空间管理” 从上到下分为4个模块：基础信息，磁盘空间趋势及分布，单日磁盘空间分布，库表分析

## 基础信息

页面顶部展示了当前数据库空间的基础信息，包括：“近30天日均增长量”，“剩余磁盘空间”，”预估可用天数“；

![image](/images/space-manage-030.png)

## 磁盘空间趋势及分布

磁盘空间趋势及分布模块直观的展示了当前实例近30天的磁盘使用空间和日志空间使用情况。

![image](/images/space-manage-040.png)

## 单日磁盘空间分布

单日磁盘空间分布以饼图的方式展示了实例中各个数据库的磁盘空间占用情况。

![image](/images/space-manage-050.png)

## 库表分析

库表分析分为4个模块：Top50表，Top50库，库表检索， 库表订阅。

### Top50表

切换到“Top50表”功能页，选择排序条件， 点击“采集数据”按钮，即可实时采集和计算当前实例中的表信息，并返回占用空间最大的前50个表。

注意：若实例库表较多或访问压力较大时，可能会造成业务出现少量延时，建议在业务低峰期采集。

![image](/images/space-manage-060.png)

一段时间后，数据采集完成，即可在列表页查看。

![image](/images/space-manage-070.png)

点击列表页右侧“操作”栏的“查看”按钮，可以查看该表的“字段”和”索引“信息。

![image](/images/space-manage-080.png)
![image](/images/space-manage-090.png)
![image](/images/space-manage-100.png)

点击列表页右侧“操作”栏的“订阅”按钮，订阅后将记录近30天的空间使用数据。可以在“库表订阅”功能页查看已订阅的库表信息。

![image](/images/space-manage-110.png)

### Top50库

功能与Top50表相同，不同是采集数据的对象是库而不是表。

![image](/images/space-manage-120.png)

点击列表页右侧“操作”栏的“订阅”按钮，订阅后将记录近30天的空间使用数据。对于已订阅的库，操作栏中可以点击”查看“按钮，查看已经收集到的空间使用数据。可以查看该库的“近30天磁盘”，“空间占用”，“物理文件大小”等相关信息。

![image](/images/space-manage-130.png)
![image](/images/space-manage-140.png)
![image](/images/space-manage-150.png)

### 库表检索

切换到“Top50表”功能页，在“库检索”，“表检索”输入对应的库名和表名，点击“查询”按钮，即可查看对应的库表信息。

![image](/images/space-manage-160.png)

如检索的时候仅输入库名，则查询的是对应数据库的信息。

![image](/images/space-manage-170.png)

同样，在操作栏中也支持订阅该库表。

### 库表订阅

切换到“库表订阅”功能页，可以看到当前订阅的库表，点击对应卡片即可查看具体信息。

![image](/images/space-manage-180.png)

对于已订阅的库表，将会以趋势图的方式展示自订阅后第二天0点起的近30天空间使用数据。

![image](/images/space-manage-190.png)

也可以点击卡片右侧的删除按钮，取消对该库表的订阅。

![image](/images/space-manage-200.png)
