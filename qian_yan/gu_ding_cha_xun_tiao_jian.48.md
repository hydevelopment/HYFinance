## 固定查询条件

### ****5.3.1、概述**** {#5-3-1}

报表中的固定查询条件，可以通过设置固定查询条件设置进入报表时，列表中的数据按设置的条件显示。

### ****5.3.2、应用场景说明**** {#5-3-2}

设置一个报表默认只显示一些符合条件的数据时，在可以通过报表的固定查询条件来设置默认列表中按设置的条件显示数据。如下图中，待验证缺陷列表中只显示fixed的数据。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\6071](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### ****5.3.3、功能说明**** {#5-3-3}

1、通过在【后台应用中心】→【建模引擎】→【报表】找到对应的报表在基础也设值固定查询条件。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\6073](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）在固定查询条件框输入sql查询条件作为报表固定查询条件。

2）固定查询条件格式表单主表表名的别名为a，查询条件的格式为: a.a = &#039;1&#039; and a.b = &#039;3&#039; and a.c like &#039;%22%&#039;。

2、设置固定条件后，前台报表列表只会结合设值的报表查询条件和固定查询条件进行显示。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\6074](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### ****5.3.4、实施注意**** {#5-3-4}

1、在写固定查询条件时，要按照参考数据库中存的值写。

2、固定查询条件支持变量参数如当前用户当前日期等 具体如下//  当前操作者 $UserId$

//  当前操作者部门$DepartmentId$

//  当前操作者部门（包含下级部门）$AllDepartmentId$

//  当前操作者分部$SubcompanyId$

//  当前操作者分部（包含下级分部）$AllSubcompanyId$

//  当前日期$date$