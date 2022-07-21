---
{
    "title": "Doris错误代码表",
    "language": "zh-CN"
}

---

<!-- 
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

# Doris错误代码表

| 错误码 | 错误信息                                                     |
| :----- | :----------------------------------------------------------- |
| 1005   | 创建表格失败，在返回错误信息中给出具体原因                   |
| 1007   | 数据库已经存在，不能创建同名的数据库                         |
| 1008   | 数据库不存在，无法删除                                       |
| 1044   | 数据库对用户未授权，不能访问                                 |
| 1045   | 用户名及密码不匹配，不能访问系统                             |
| 1046   | 没有指定要查询的目标数据库                                   |
| 1047   | 用户输入了无效的操作指令                                     |
| 1049   | 用户指定了无效的数据库                                       |
| 1050   | 数据表已经存在                                               |
| 1051   | 无效的数据表                                                 |
| 1052   | 指定的列名有歧义，不能唯一确定对应列                         |
| 1053   | 为Semi-Join/Anti-Join查询指定了非法的数据列                  |
| 1054   | 指定的列在表中不存在                                         |
| 1058   | 查询语句中选择的列数目与查询结果的列数目不一致               |
| 1060   | 列名重复                                                     |
| 1064   | 没有存活的Backend节点                                        |
| 1066   | 查询语句中出现了重复的表别名                                 |
| 1094   | 线程ID无效                                                   |
| 1095   | 非线程的拥有者不能终止线程的运行                             |
| 1096   | 查询语句没有指定要查询或操作的数据表                         |
| 1102   | 数据库名不正确                                               |
| 1104   | 数据表名不正确                                               |
| 1105   | 其它错误                                                     |
| 1110   | 子查询中指定了重复的列                                       |
| 1111   | 在Where从句中非法使用聚合函数                                |
| 1113   | 新建表的列集合不能为空                                       |
| 1115   | 使用了不支持的字符集                                         |
| 1130   | 客户端使用了未被授权的IP地址来访问系统                       |
| 1132   | 无权限修改用户密码                                           |
| 1141   | 撤销用户权限时指定了用户不具备的权限                         |
| 1142   | 用户执行了未被授权的操作                                     |
| 1166   | 列名不正确                                                   |
| 1193   | 使用了无效的系统变量名                                       |
| 1203   | 用户使用的活跃连接数超过了限制                               |
| 1211   | 不允许创建新用户                                             |
| 1227   | 拒绝访问，用户执行了无权限的操作                             |
| 1228   | 会话变量不能通过SET GLOBAL指令来修改                         |
| 1229   | 全局变量应通过SET GLOBAL指令来修改                           |
| 1230   | 相关的系统变量没有缺省值                                     |
| 1231   | 给某系统变量设置了无效值                                     |
| 1232   | 给某系统变量设置了错误数据类型的值                           |
| 1248   | 没有给内联视图设置别名                                       |
| 1251   | 客户端不支持服务器请求的身份验证协议；请升级MySQL客户端      |
| 1286   | 配置的存储引擎不正确                                         |
| 1298   | 配置的时区不正确                                             |
| 1347   | 对象与期望的类型不匹配                                       |
| 1353   | SELECT和视图的字段列表具有不同的列数                         |
| 1364   | 字段不允许NULL值，但是没有设置缺省值                         |
| 1372   | 密码长度不够                                                 |
| 1396   | 用户执行的操作运行失败                                       |
| 1471   | 指定表不允许插入数据                                         |
| 1507   | 删除不存在的分区，且没有指定如果存在才删除的条件             |
| 1508   | 无法删除所有分区，请改用DROP TABLE                           |
| 1517   | 出现了重复的分区名字                                         |
| 1567   | 分区的名字不正确                                             |
| 1621   | 指定的系统变量是只读的                                       |
| 1735   | 表中不存在指定的分区名                                       |
| 1748   | 不能将数据插入具有空分区的表中。使用“ SHOW PARTITIONS FROM  tbl”来查看此表的当前分区 |
| 1749   | 表分区不存在                                                 |
| 5000   | 指定的表不是OLAP表                                           |
| 5001   | 指定的PROC路径无效                                           |
| 5002   | 必须在列置换中明确指定列名                                   |
| 5003   | Key列应排在Value列之前                                       |
| 5004   | 表至少应包含1个Key列                                         |
| 5005   | 集群ID无效                                                   |
| 5006   | 无效的查询规划                                               |
| 5007   | 冲突的查询规划                                               |
| 5008   | 数据插入提示：仅适用于有分区的数据表                         |
| 5009   | PARTITION子句对于INSERT到未分区表中无效                      |
| 5010   | 列数不等于SELECT语句的选择列表数                             |
| 5011   | 无法解析表引用                                               |
| 5012   | 指定的值不是一个有效数字                                     |
| 5013   | 不支持的时间单位                                             |
| 5014   | 表状态不正常                                                 |
| 5015   | 分区状态不正常                                               |
| 5016   | 分区上存在数据导入任务                                       |
| 5017   | 指定列不是Key列                                              |
| 5018   | 值的格式无效                                                 |
| 5019   | 数据副本与版本不匹配                                         |
| 5021   | BE节点已离线                                                 |
| 5022   | 非分区表中的分区数不是1                                      |
| 5023   | alter语句中无任何操作                                        |
| 5024   | 任务执行超时                                                 |
| 5025   | 数据插入操作失败                                             |
| 5026   | 通过SELECT语句创建表时使用了不支持的数据类型                 |
| 5027   | 没有设置指定的参数                                           |
| 5028   | 没有找到指定的集群                                           |
| 5030   | 某用户没有访问集群的权限                                     |
| 5031   | 没有指定参数或参数无效                                       |
| 5032   | 没有指定集群实例数目                                         |
| 5034   | 集群名已经存在                                               |
| 5035   | 集群已经存在                                                 |
| 5036   | 集群中BE节点不足                                             |
| 5037   | 删除集群之前，必须删除集群中的所有数据库                     |
| 5037   | 集群中不存在这个ID的BE节点                                   |
| 5038   | 没有指定集群名字                                             |
| 5040   | 未知的集群                                                   |
| 5041   | 没有集群名字                                                 |
| 5042   | 没有权限                                                     |
| 5043   | 实例数目应大于0                                              |
| 5046   | 源集群不存在                                                 |
| 5047   | 目标集群不存在                                               |
| 5048   | 源数据库不存在                                               |
| 5049   | 目标数据库不存在                                             |
| 5050   | 没有选择集群，请输入集群                                     |
| 5051   | 应先将源数据库连接到目标数据库                               |
| 5052   | 集群内部错误：BE节点错误信息                                 |
| 5053   | 没有从源数据库到目标数据库的迁移任务                         |
| 5054   | 指定数据库已经连接到目标数据库，或正在迁移数据               |
| 5055   | 数据连接或者数据迁移不能在同一集群内执行                     |
| 5056   | 不能删除数据库：它被关联至其它数据库或正在迁移数据           |
| 5056   | 不能重命名数据库：它被关联至其它数据库或正在迁移数据         |
| 5056   | 集群中BE节点不足                                             |
| 5056   | 集群内已存在指定数目的BE节点                                 |
| 5059   | 集群中存在处于下线状态的BE节点                               |
| 5062   | 不正确的群集名称（名称'default_cluster'是保留名称）          |
| 5063   | 类型名不正确                                                 |
| 5064   | 通用错误提示                                                 |
| 5063   | Colocate功能已被管理员禁用                                   |
| 5063   | colocate数据表不存在                                         |
| 5063   | Colocate表必须是OLAP表                                       |
| 5063   | Colocate表应该具有同样的副本数目                             |
| 5063   | Colocate表应该具有同样的分桶数目                             |
| 5063   | Colocate表的分区列数目必须一致                               |
| 5063   | Colocate表的分区列的数据类型必须一致                         |
| 5064   | 指定表不是colocate表                                         |
| 5065   | 指定的操作是无效的                                           |
| 5065   | 指定的时间单位是非法的，正确的单位包括：HOUR / DAY / WEEK / MONTH |
| 5066   | 动态分区起始值应该小于0                                      |
| 5066   | 动态分区起始值不是有效的数字                                 |
| 5066   | 动态分区结束值应该大于0                                      |
| 5066   | 动态分区结束值不是有效的数字                                 |
| 5066   | 动态分区结束值为空                                           |
| 5067   | 动态分区分桶数应该大于0                                      |
| 5067   | 动态分区分桶值不是有效的数字                                 |
| 5066   | 动态分区分桶值为空                                           |
| 5068   | 是否允许动态分区的值不是有效的布尔值：true或者false          |
| 5069   | 指定的动态分区名前缀是非法的                                 |
| 5070   | 指定的操作被禁止了                                           |
| 5071   | 动态分区副本数应该大于0                                      |
| 5072   | 动态分区副本值不是有效的数字                                 |
| 5073   | 原始创建表stmt为空                                           |
| 5074   | 创建历史动态分区参数：create_history_partition无效，期望的是：true或者false |
| 5076   | 指定的保留历史分区时间段为空                           |
| 5077   | 指定的保留历史分区时间段无效                            |
| 5078   | 指定的保留历史分区时间段必须是成对的时间             |
| 5079   | 指定的保留历史分区时间段对应位置的第一个时间比第二个时间大（起始时间大于结束时间）  |
