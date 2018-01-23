## 树

### ****6.7.1、概述**** {#6-7-1}

通过以下2个例子讲解表单建模中的树形如何配置，有了此2个案例的配置基础之后 再深层介绍树形配置页面的功能点介绍

### ****6.7.2、案例一（组织结构树）**** {#6-7-2}

利用树形功能配置出组织结构树，此树是有四部分组成的顶部根节点，根节点下是分部，分部下是部门，部门下是人员。

此树中涉及到表单有

分部表名：HrmSubCompany主建：id上级：SUPSUBCOMID 显示名称：SUBCOMPANYNAME

链接目标地址：/hrm/company/HrmDepartment.jsp?subcompanyid=$ID$

部门：表名：hrmdepartment 主建：id上级：SUPDEPID 显示名称：DEPARTMENTNAME

链接目标地址：/hrm/company/HrmDepartmentDsp.jsp?id=$id$

人员：表名：hrmresource主建：id上级：MANAGERID显示名称：LASTNAME

链接目标地址：/hrm/resource/HrmResource.jsp?id=$id$

**展现效果：**

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407059](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**如何配置**

1、在系统【后端应用中心】→【建模引擎】---&gt;点击某个应用然后点击查询tab页页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407062](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图1）

2、点击（图1）页面右键 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407064](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图2）

3、点击（图2）页面上的新建按钮出来的页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407065](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图3）

4、在（图3）页面填写数据如下保存之后效果如下

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407071](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图4）

此时右键点击预览按钮出来的效果如下图（此时配置出树的顶部）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407087](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

5、点击（图4）页面右键 新建树节点按钮 出来页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407091](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图5）

此页面填写好数据之后效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407092](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

6、此页面保存之后 再返回到【树形设置：基本信息】页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407095](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图6）

此时再右键预览的时候显示效果如下（此时配置顶部下的分部）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407096](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

7、在（图6）页面上右键 点击 新建树节点按钮 如（图5）填写完数据之后 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407098](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

此页面保存之后再返回到【树形设置：基本信息】页面 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407115](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

8、此时在此页面右键 点击预览按钮 页面显示效果如下（此时配置的是分部下的部门）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407121](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

9、在以下页面中再右键 点击【新建树节点】按钮 点击此按钮显示的页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407122](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

在上图中填写完信息保存之后的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407123](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

此页面保存之后再返回到【树形设置：基本信息】页面 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407125](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

点击此页面上的右键预览按钮出来的效果如下图（此时配置的是部门下的人员）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407126](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

11、以上配置完成之后 在如下图的页面 右键 点击创建菜单按钮 配置树形的前台菜单 配置完之后效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407127](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### ****6.7.3、案例二（模块配置的树）**** {#6-7-3}

利用表单建模中搭建的模块配置出树形

比如目前系统中有以下几个模块

研发人员模块

任务模块

此两个模块的表单利用自定义浏览框关联的关系是在任务模块关联的表单中有个研发人员字段 存放的是研发人员模块中的内容。

**需要展现的效果如下**

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407132](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**如何配置**

有了案例一的配置基础之后我们就简化一些配置步骤 具体如下图

1、在【后端应用中心】【建模引擎】-“树形”页面右键新建树 新建完之后效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407138](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图11）

2、在上图页面上右键 点击 新建树节点按钮 （二级树节点） 比如取名为研发测试人员 填写信息如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407141](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

3、建完之后返回到树形的基本设置页面 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407142](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

4、在此页面上右键预览效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407146](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

配置菜单发布前台的步骤这里不再详细描述

**四、树形配置页面的功能点介绍**

有了案例一，案例二中的树形配置基础之后接下来我们详细介绍下 树形配置页面上的各个属性表示什么样的功能。

详情见

1、**《导航树》**

2、**《树形浏览框》**

3、树形涉及到的功能点如下

**《复制树形》**

**《树形根节点主键值及treesqlwhere参数》**