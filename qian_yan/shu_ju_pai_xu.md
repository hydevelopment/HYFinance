## 数据排序

### ****4.9.1、概述**** {#4-9-1}

可以通过设置排序和默认排序优先级设置查询列表中数据的排序方式。

### ****4.9.2、应用场景说明**** {#4-9-2}

通过查询列表的数据排序功能，设置查询列表默认排序或者设置指定字段可以前台进行排序，通过排序功能可以更方便的预览列表中数据。如下图：

**![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\5719](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)**

### ****4.9.3、功能说明**** {#4-9-3}

1、通过在【后台应用中心】→【建模引擎】→【查询】在对应的查询列表的字段定义中通过设置排序和默认排序优先级设置查询列表数据排序的功能。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\5717](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）排序：排序中包含是、否、默认升序、默认降序四个选项。选择是时，前台可以点击对应的字段标题进行手动排序；选否时则不能排序；选择默认升序后，前台查询列表数据会默认按照该字段数据进行升序排序，可以通过手动点击对应字段标题进行手动排序；选择默认降序时，前台查询列表数据会默认按照该字段数据进行降序排序，可以通过手动点击对应字段你标题进行手动排序。

2）默认排序优先级：通过填写数字设置默认排序字段的优先级，仅在排序选择默认升序或者默认降序时生效。

2、设置了排序时，前台会按照排序设置进行排序，也可以手动点击标题进行排序。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\5719](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### ****4.9.4、实施注意**** {#4-9-4}

1、排序优先级只有在排序选择默认升序或者默认降序时才可以设置。

2、支持排序字段的类型有：单文本、整数、浮点数、金额转换、金额千分位、选择框、浏览框（单选）。

3、前台排序时是按照数据库中存的值进行排序，如选择框和浏览框是按照0、1、2…和浏览框的id进行排序，而不是按照浏览框和选择框显示的值排序。

4、如果有设置默认排序，点击标题时，会按照点击标题对应的字段进行排序。