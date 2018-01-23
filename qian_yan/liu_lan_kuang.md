## 浏览框

### ****6.1.1概述**** {#6-1-1}

自定义浏览框可以理解为是在表单引擎中的表与表关联的一个桥梁。比如 利用表单引擎搭建了一个车辆管理

驾驶员信息是一张表单  车辆信息是一张表单  车辆信息卡片中有个字段名为司机 关联的是驾驶员信息表单中

一条或者多条数据 那么司机这个字段是如何关联我们驾驶员卡片的信息 这个就需要通过我们的自定义浏览框功能

作为一个桥梁把两者联系起来。

### ****6.1.2、前端效果**** {#6-1-2}

要实现概述中描述的需求的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\10931](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### ****6.1.3、功能配置说明**** {#6-1-3}

要实现上面的需求 接下来的配置 是车辆信息模块和驾驶员信息模块 在表单引擎中已经搭建完 此些模块的搭建步骤 我们不做阐述。接下来的步骤是在此基础上操作的。

在系统【后端应用中心】→【建模引擎】---&gt;点击某个应用然后 点击浏览框tab页 页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\10934](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

点击上图中的“字段定义”tab页  设置自定义浏览框显示的字段 具体如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\10948](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

上图配置完之后 然后再回到“基础”tab页 然后再右键 点击“创建浏览框”按钮

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\10968](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

上图创建浏览框按钮之后 我们可以在“浏览框列表”tab页 看到创建浏览框按钮的标识 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\10970](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                                              图（5）

上述配置完之后 接下来 我们到车辆信息的表单里面去 车辆信息表单字段页面司机字段如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\10971](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

上述配置完之后 我们就可以看到“二、前端效果”中的效果。 如果要设置成多选的浏览框 只需要将上图中的 自定义单选 选择为自定义多选即可。