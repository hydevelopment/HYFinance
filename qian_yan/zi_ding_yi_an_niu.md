## 自定义按钮

### ****4.14.1、概述**** {#4-14-1}

定义查询列表上数据的自定义按钮具体效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1401041](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### ****4.14.2、功能说明**** {#4-14-2}

在系统【后端应用中心】→【建模引擎】---&gt;点击某个应用然后点击查询tab页页面下的“自定义按钮”如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1401042](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图1）

在（图1）页面上右键点击“新建”按钮出现的页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1401070](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

页面属性说明：

名称：自定义按钮的名称

链接目标方式：点击此按钮跳转的路径或者执行的方法。

*   手动输入：定义按钮执行的方法
*   链接：定义按钮跳转的路径。

当链接目标方式选择手动输入时：

*   javascript方法名：定义js方法名。命名规范为：javascript:onUrl();
*   javascript方法参数：js方法中传递的参数名。这个是字段的列名
*   javascript方法体：编写js方法的逻辑代码。方法体命名规范：function onUrl（id,params）{}

当链接目标方式选择链接时

*   链接打开方式：打开路径的方式。TAB页:新的tab页打开，弹出框：以弹出框的方式打开。
*   链接目标参数id：传递路径的参数名称
*   链接目标参数field：传递路径参数名称对应的值可以填写字段列名就表示取这个字段列的值作为参数的值。

接口路径：定义此按钮显示的接口代码。

是否显示：勾选表示此按钮显示不勾选表示不显示

描述：此按钮的说明

显示顺序：此按钮的显示顺序（图1）列表页面上数据按照此显示顺序的升序排序。

当链接目标方式：手动输入时例子如下：

1、后台配置页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1401071](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

Javascript方法参数：填写字段的列名如果有多个则以逗号隔开。

2、前端显示效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1401077](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

当链接目标方式：链接时例子如下：

1、后台配置页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1401079](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

链接目标参数id：自定义的一个参数名称名为objname

链接目标参数field:为查询列表关联表单中的字段名。bh为编号字段。

2、前端显示效果如下

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1401083](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

自定义接口路径中的代码格式如下图：

| package weaver.formmode.interfaces.action;import weaver.formmode.interfaces.PopedomCommonAction;import weaver.formmode.setup.ModeRightInfo;public class TestAction implements PopedomCommonAction {@Overridepublic String getIsDisplayOperation(String uid, String billid) {ModeRightInfo modeRightInfo = new ModeRightInfo();    modeRightInfo.writeLog(&quot;==zdystart====&quot;);modeRightInfo.writeLog(&quot;uid：&quot;+uid);modeRightInfo.writeLog(&quot;billid:&quot;+billid);    modeRightInfo.writeLog(&quot;==zdyend===&quot;);    if (&quot;1&quot;.equals(billid)){     return &quot;false&quot;;    } else {return &quot;true&quot;;}}} |
| --- |

说明：需要实现PopedomCommonAction接口。该接口中有一实现方法getIsDisplayOperation，参数userid和billid，返回值为”true”或者”false”字符串。如果在接口路径中不输入，或者输入有误，默认返回true，也就是默认显示自定义按钮。