## 功能说明

通过进入【后端应用中心】→【建模引擎】→【提醒】，切换到需要新建提醒对应的应用下，可以查看已有提醒，也可以新建提醒，当对应应用下没有提醒时，会直接显示新建提醒页面。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407921](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

提醒类型分为即时提醒、到期提醒、循环提醒，如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407922](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）即时提醒：即时提醒是只在新建模块数据保存时，符合提醒条件的数据会即时发送提醒。

2）到期提醒：到期提醒是指会根据设置的提醒条件，结合定时器设置以及到期时间和时间增量设置对应时间发送提醒。

3）循环提醒：循环提醒是指针对符合提醒条件发送的数据，会根据定时器设置循环发送提醒。

**A、即时提醒**

1、选择提醒类型为即时提醒，设置即时提醒的基本信息和提醒信息后保存。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407940](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2、设置提醒的基本信息，如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407949](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）名称：设置提醒的名称。

2）是否启用：设置是否启用该提醒，勾选启用，不勾选不启用。

3）提醒类型：设置提醒类型。

4）表单名称：选择需要设置提醒对应的表单。

5）模块名称：选择需要设置提醒对应的模块，可以选择已选表单关联的所有可用模块。

3、设置提醒的提醒信息。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407953](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）提醒方式：设置是短信提醒还是邮件提醒。

2）提醒条件：设计提醒需要满足的条件，可以通过字段或者sql条件设置。

3）提醒内容：设置提醒内容，可以通过文本内容或者java类型设置，设置文本时，可以通过选择字段变量将变量值带到提醒内容中。

4）提醒人员：设置提醒接收的人员，通过设置多种类型过滤接收提醒的人员。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407972](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

选择：根据提醒人员设置的类型，选择对应的内容。

安全级别：根据提醒人员选择的类型，可以设置安全级别，选择分部、部门、角色、所有人时可以通过设置的安全级别过滤接收提醒的人员，如选择的分部中安全级别大于等于10的人员接收提醒信息。

提醒方式可以设置短信提醒和邮件提醒，设置短信提醒时，需要设置短信发送人；设置邮件提醒时需要设置邮件标题。

短信提醒：设置短信提醒时，需要设置短信发送人，如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407974](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

邮件提醒：设置邮件提醒时，需要设置邮件标题，如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407976](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**B、到期提醒**

选择提醒类型为到期提醒，则会结合定时器运行在设置的到期时间进行提醒。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407980](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

设置基本信息，除到期时间和时间增量，其他设置同即时提醒。详见即时提醒设置基本信息

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407987](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）到期时间：可以通过设置常量（固定日期、时间）或者通过字段，设置表单中字段作为到期时间。

2）时间增量：可是设置是提前还是延迟提醒，可以设置整数常量或者是选择表单中的整数字段。

例如：如下设置则表示在2015-05-15 19：59提前5分钟发送相应的提醒，则会在19：54针对符合条件的模块数据发送提醒，如果设置的字段时，则会在对应字段的日期、时间按照时间增量设置进行提醒。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407989](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

设置提醒信息，到期提醒提醒信息设置同即时提醒。详见即时提醒提醒信息设置。

设置定时器。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407992](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：通过启用定时器会按照设置的时间发送提醒。

1）定期器触发方式：可以选择简单规则或者是表单式的方式设置定时器，设置简单规则时需要设置定期器

2）运行频率和定时器循环周期；设置表达式时，则可以通过定时器表达式设置定时器启用的规则。

3）定时器运行频率（简单规则）：设置定时器运行的频率。

4）定时器循环周期（简单规则）：设置定时器的循环周期。

5）定时器表达式（表达式）：定时器触发方式为表达式时，通过定时器表达式设置启用定时器。表达式格式为：[秒] [分] [小时] [日] [月] [周] [年]，如下图则表示每天的12:00:00触发定时器。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407993](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**C、循环提醒**

1、提醒类型设置为循环提醒时，则根据定时器运行，循环提醒符合条件的数据。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407994](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

设置循环提醒基本信息，与即时提醒相同。详见即时提醒设置基本信息。

提醒信息设置同即时提醒。详见即时提醒提醒信息设置。

定时器设置，同到期提醒，详见到期提醒定时器设置。