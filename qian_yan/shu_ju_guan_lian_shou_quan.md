## 数据关联授权

### ****2.9.1、概述**** {#2-9-1}

通过数据关联授权功能，在模块中存在客户、多客户、文档、多文档、自定义单选、自定义多选、自定义树形单选、自定义树形多选浏览框字段时，可以设置字段进行关联授权，在查看模块数据时，即使没有浏览框引用的对应数据权限，也可以在建模卡片中查看相应的数据。

### ****2.9.2、应用场景说明**** {#2-9-2}

例如，当用户有模块A的数据权限，但是没有模块B的权限，当模块A中存在浏览框引用模块B的数据时，当不开启关联授权时，用户点击浏览框的链接查看模块B的数据时，会提示无权限，通过数据关联授权，则可以设置相应的字段进行关联授权，用户在在模块A的卡片信息页面，则可以点击引用了模块B数据的浏览框，查看模块B的数据。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1281662](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### 2.9.3、功能说明 {#2-9-3}

1、 通过进入【后端应用中心】→【建模引擎】→【模块】，在对应模块的数据关联授权tab页，可以设置需要关联授权的字段。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1281664](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1） 列表中会显示出该模块对应表单主表和明细表中可以设置数据关联授权的字段（自定义单选、自定义多选、文档、多文档、客户、多客户类型的浏览框字段支持数据关联授权）。

2） 是否授权：可以设置该字段是否需要授权。

3） 布局：针对自定义单选和自定义多选类型的浏览框，可以设置浏览框引用的模块数据显示的布局。

4） 布局级别：针对设置布局时，设置布局的级别，点击链接查看时，如果能找到多个布局，则按布局级别来加载对应布局，数字越小，优先级越高，显示布局级别值最小的布局。

2、 对应字段开启授权后，只要有对应模块数据的权限，在模块卡片页面中就可以点击链接查看相关信息。如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1281665](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)3、 文档、多文档、客户、多客户、自定义树形单选、自定义树形多选字段也是一样。

### ****2.9.4、实施注意**** {#2-9-4}

1、 支持关联授权的浏览框类型有：自定义单选、自定义多选、自定义树形单选、自定义树形多选、文档、多文档、客户、多客户。

2、 只有自定义单选、和自定义多选浏览框字段可以设置布局。

3、 自定义树形单选、自定义树形多选，链接目标模块存在多个布局时，加载默认布局。

4、 数据关联授权只支持在卡片页面点击链接查看，在其他地方点击链接权限跟随对应的模块共享权限，如没有目标模块权限，则提示无权限。

5、 关闭对应字段关联授权时，不进行授权，没有权限时，点击会提示无权限。

6、 主表和明细表中的字段都可以设置关联授权。

7、 通过默认共享和前端非默认共享后，对应的用户都可以查看开启关联授权的字段对应的信息。