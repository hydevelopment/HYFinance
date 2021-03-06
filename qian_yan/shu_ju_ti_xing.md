## 数据提醒

### ****3.4.1、概述**** {#3-4-1}

数据提醒功能是设置表单中指定字段在前台输入重复数据的校验，当前台输入重复数据时，会提醒用户不符合数据唯一性校验。

### ****3.4.2、应用场景说明**** {#3-4-2}

有需求是 我需要在某个卡片上验证某个字段的唯一性 比如很常见的 我们的身份证，手机号都是唯一 不允许有重复的 那么在前端这2个字段输入值的时候 我们就可以利用数据提醒功能来验证这2个字段的唯一性。

### ****3.4.3、功能说明**** {#3-4-3}

表单建模，表单字段设置中可以设置字段的数据提醒，支持设置单文本、整数、浮点数、金额千分位类型的字段（如下图）。![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\6374](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

支持设置数据提醒的字段类型有：

*   单行文本-文本
*   单行文本-整数
*   单行文本-浮点数
*   单行文本-金额千分位

1.1 设置方法

表单建模，在后台设置字段的数据提醒，在对应字段勾选数据提醒，在前台新建数据保存时，会对数据进行唯一性校验。

在表单字段设置中，可以设置数据提醒的字段会显示对应的复选框。

*   勾选：勾选时在前台会对对应的字段进行唯一性校验。
*   不勾选：不勾选时，在前台不会对对应的字段进行唯一性校验。

1.2.1 启用数据提醒功能。

对应的字段启用了数据提醒时，在前台新建数据时，输入重复的数据，保存时，会弹出提示，并标识出不符合的数据（如下图）。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\6379](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

1.2.2 不启用数据提醒功能。

将对应字段的数据提醒去勾选时候，在前台输入重复的数据，也可以正常保存，不会进行唯一性校验。

### ****3.4.4、实施注意**** {#3-4-4}

1、数据提醒功能是一表单为维度进行校验的，多个模块引用相同的表单，只要表单中存在重复的数据，在开启数据提醒功能时则会进行校。

2、数据提醒功能支持的字段有单文本、整数、浮点数、金额千分位。

3、虚拟表单和明细表中的字段是不支持此功能。