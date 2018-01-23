## 获取表单数据总数

### ****10.4.1、方法介绍**** {#10-4-1}

方法：getAllModeDataCount(**int** modeId,**int** userId, String conditions,String right);

输入参数：@param modeId 表单ID@param userId 用户ID@param conditions 查询条件@param right （y/n） 是否受权限控制

输出参数：int: 表单总数

### ****10.4.2、实例效果**** {#10-4-2}

实例调用如下

| /** |
| --- |

执行后效果：

331

表示 此用户有权限看到此表单的数据为331条数据。