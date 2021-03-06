## 快捷搜索字段

### ****6.6.1、概述**** {#6-6-1}

通过快捷搜索字段功能，可以实现在浏览框的方框中输入内容然后过滤出浏览框框列表数据，直接选择需要的数据，实现快捷选择数据的功能。

### ****6.6.2、应用场景说明**** {#6-6-2}

当浏览框选择数据时，点击浏览框图标进入浏览框列表中找对应的数据，当数据量大的时候比较难找，通过快捷搜索功能可以输入匹配的字符然后过滤出浏览框数据列表，从中选择即可。

如选择图书时，直接从图书列表中选择数据比较多比较麻烦，可以直接在浏览框的输入框中输入内容，则会过滤出对应的数据，选择自己需要的数据即可。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\7493](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### ****6.6.3、功能说明**** {#6-6-3}

1、通过【后台应用中心】→【建模引擎】→【浏览框】在对应的浏览框字段定义页面，通过设置快捷搜索字段，如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\7495](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）通过设置快捷搜索字段，在前台浏览框输入框中输入该字段相关内容时，则会过滤出数据供选择。

2）可设置快捷搜索字段类型有：单文本、多文本、整数、浮点数、金额转换、金额千分位。

3）可设置多个快捷搜索字段，设置后，输入内容会过滤出都符合条件的数据，但是列表中是显示该条数据对应的标题字段的内容。

2、浏览框启用快捷搜索前台显示效果如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\7496](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### ****6.6.4、实施注意**** {#6-6-4}

1、可以设置多个快捷搜索字段，设置多个字段时，前台过滤列表显示的是过滤出的列表对应的标题字段信息。

2、支持设置快捷搜索字段的字段类型有：单文本、多文本、整数、浮点数、金额转换、金额千分位。

3、如果修改过浏览框的标题字段（链接字段）信息，则需要重新初始化被应用浏览框标识的信息，否则过滤列表显示可能与设置不一致。