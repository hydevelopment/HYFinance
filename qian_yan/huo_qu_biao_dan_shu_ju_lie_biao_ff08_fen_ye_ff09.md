## 获取表单数据列表（分页）

### 10.6.1、方法介绍 {#10-6-1}

方法：getAllModeDataList (21, 1, 10, 0, 1, &quot;&quot;,&quot;n&quot;,&quot;Y&quot;);

输入参数：

@param modeId 表单ID@param pageNo 当前页数@param pageSize 每页记录数@param recordCount 记录总数（小于等于0时自动计算记录总数）@param userid 当前用户@param conditions 查询条件@param right （y/n） 是否受权限控制@param isReturnDetail （y/n） 是否返回明细表数据

输出参数：

String: 表单数据列表（分页）

### 10.6.2、实例效果 {#10-6-2}

实例效果如下

| **publicvoid** getAllModeDataList(){ |
| --- |

 效果如下

| &lt;?xmlversion=&quot;1.0&quot;encoding=&quot;UTF-8&quot;?&gt; |
| --- |

1.  【新功能】