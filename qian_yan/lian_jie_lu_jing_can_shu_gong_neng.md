## 链接路径参数功能

### ****4.6.1、概述**** {#4-6-1}

链接路径参数功能是指链接的路径获取字段的值作为url路径中参数的值。

### 4.6.2、功能说明 {#4-6-2}

在系统【后端应用中心】→【建模引擎】---&gt;点击某个应用然后点击查询tab页页面下的“字段定义”页面中的链接路径编写参数值 具体 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1401562](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）标题字段支持单文本、整数、浮点数、金额转换、金额千分位、选择框类型字段。

2）默认勾选时，会带出模块卡片链接地址，可以自定义编辑链接地址为流程查看地址或者自定义的链接地址，地址中可以通过$字段名$的格式取当前表单字段的值。

3）设置链接地址示例（红色字体部分为动态取当前表单字段值格式）：

表单建模：

/formmode/view/AddFormMode.jsp?type=$type$&amp;modeId=$modeId$&amp;formId=$formId$&amp;billid=$billid$&amp;opentype=$opentype$&amp;customid=$customid$&amp;viewfrom=$viewfrom$&amp;bh=$bh$

工作流：/workflow/request/ViewRequest.jsp?requestid=$requestId$&amp;isovertime=0&amp;bh=$bh$

其他自定义：http://www.baidu.com?bh=$bh$

设置后，点击标题字段链接可以链接到对应的地址并且解析出对应参数的值 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1401565](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

注意：链接字段参数不支持带格式文本字段。