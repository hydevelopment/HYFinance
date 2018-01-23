## 【查询相关】

### 11.2.1、主子表数据显示 {#11-2-1}

**一、概述**

当模块表单中存在明细表时，查询中可以选择一个子表，字段定义中可以设置显示主表和明细表字段。

**二、应用场景说明**

当需要在列表中显示主表字段和明细表字段时，可以在设置查询列表时选择相应的子表，然后在字段定义中勾选需要显示的字段,实现在列表中显示主表和明细表的数据。应用实例如下图：

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\5914](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、功能说明**

1、通过在【后台应用中心】→【建模引擎】→【查询】在指定的查询列表中选择需要显示的子表。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\5833](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

子表可以选择该表单中存在的所有明细表中的一个，选择后字段定义中会显示选择的明细表的字段，勾选标题列对应字段则可以设置前台显示对应字段。

2、在字段定义中设置要显示的字段。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\5835](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

选择子表后，需要在字段定义中选择要显示的主表和明细表字段。

3、前台显示效果。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\5836](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：当列表字段定义有配置主表和明细表字段时，前台会按照明细表的数量显示数据，主表字段显示明细表对应的主表记录信息。

**四、实施注意**

1、需要在查询基础页面选择子表后，字段定义中才能看到对应的明细表字段。

2、设置主子表查询时，查询列表中的数量以子表记录计算。

### 11.2.2、未读，反馈标识 {#11-2-2}

**一、概述**

在查询列表标题字段增加标识，人员通过标识知道哪些列表数据未读、已读和修改

**二、应用场景说明**

查询列表中，某条表单数据中的标题字段内容后出现红色图标，表示该用户还未查看此数据，标题字段内容后出现黄色图标，表示该用户查看该条数据后，此数据又被修改过，没有任何图标，表示用户查看该数据后，该数据没有再修改过，如图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1274844](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、功能说明**

启动和不启动此功能，需要在/WEB-INF/prop/formmode.properties配置文件中添加以下代码：

#是否开启列表未读，反馈标识功能。 Y:开启  N:关闭

Enabled=N

系统默认是关闭状态，开启后的效果如图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1274845](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

开启了列表标识功能，在前台查询列表高级搜索中添加了“数据状态”搜索条件如图，勾选对应check框，搜索对应的数据

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1274846](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**四、实施注意**

1，在后台设置多个列表标题字段，在前台对应多个标题字段都可以显示图标

2，明细子表显示在查询列表，支持标识显示功能

3，门户中建模自定义查询元素，支持标识显示功能

4，引用虚拟表单创建的查询列表，不支持此功能