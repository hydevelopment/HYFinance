## 【其他相关】

### 11.5.1、明细表行复制功能 {#11-5-1}

**一、概述**

1、在后台编辑布局和新建布局可以设置此明细表是否拥有复制功能。

2、后台布局中勾选了复制 则在前端明细表右上方可以看到复制按钮。配置和使用同明细表的“新建”和“删除”按钮一样。

**二、功能说明**

在【后端应用中心】----【建模引擎】---“某个具体的模块”---下的新建布局或者编辑布局如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343390](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图1）

点击（图1）中的新建布局进去显示的页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343391](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图2）

点击（图2）页面上的“字段属性批量设置”弹出的页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343392](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图3）

在（图3）页面上勾选下红色框中的“允许复制明细”后的复选框然后保存卡片前端明细表上会出现“复制”按钮效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343393](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图4）

在（图4）中选中要复制的行然后点击“复制”按钮出现的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343394](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

### 11.5.2、e8建模附件字段权限改进 {#11-5-2-e8}

**一、概述**

1、权限页面右键添加了文档权限重构，可以查看历史数据中附件字段内容

2、在前台删除模块数据权限，查看对应文档目录附件权限也会跟着删除

3、能查看模块中附件权限，对应的文档目录也有权限查看该附件

**二、功能说明**

**A、文档权限重构**

进入【模块】-【基础】设置页面中，在“附件上传目录”中添加附件存放的文档目录保存后（如图1），

在【模块】-【权限】页面中，右键选择“文档权限重构”（如图2），默认共享权限人员可以有权限查看历史数据附件字段的内容，有模块权限人员可以在对应的文档目录中有权限查看历史数据附件字段内容

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409317](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                 （图1）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409327](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                              （图2）

B、附件字段权限

1）用户新建表单，添加附件字段内容保存后，非默认共享和默认共享权限的人员在模块中有权限查看附件字段内容，在对应的文档目录中，有权限查看附件（如图3）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409334](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                                                                  （图3）

2）在前台共享权限页面中，删除有非默认共享权限人员或者默认共享权限人员，查看对应文档目录附件权限也相应删除。（如图4）删除默认共享权限的人员保存后，文档共享权限也对应删除（如图5）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409341](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                                     （图4）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409346](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                 （图5）

**三、实施注意**

 1、在前台删除模块权限，查看对应文档目录中附件权限的权限也实时删除

2、在后台删除权限后，权限重构功能仅针对表单建模中的数据权限进行重构，文档权限重构功能是仅针对表单建模中的附件文档权限进行重构，2个功能相互独立

### 11.5.3、表单建模回复功能 {#11-5-3}

**一、概述**

通过表单建模回复功能，可以设置模块是否启用回复功能，启用回复功能后，有权限查看模块数据的人员可以对模块数据进行回复评论。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409367](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**二、功能说明**

**A、后端配置**

1、通过进入【后端应用中心】→【建模引擎】，点击设置图标。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409369](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2、开启回复评论功能后保存，第一次开启后，会初始化回复评论数据，刷新应用树后会显示回复评论应用。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409370](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

3、可以通过修改显示顺序，便于查找。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409372](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

4、第一次开启回复功能主要是初始化应用、模块、表单、布局信息。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409375](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

5、布局是初始化后，可以备份布局信息，如果需要恢复，则可以源代码内容在布局中覆盖。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409376](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

6、如果需要在回复中添加附件，需设置附件目录。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409377](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

7、开启对应模块的回复功能。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409379](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**B、前端效果**

1、开启回复功能后，在对应模块的查看页面进行回复评论。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409382](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）添加、删除、引用、回复评论。

2）提交的评论在10分钟内允许修改、删除，超过10分钟不能修改、不能删除。

3）附加功能可以引用附件、文档、客户、项目、流程内容，项目和流程的打开与对应权限相关；附件、文档、客户，只要有权限看到回复信息，则在回复页面可以点开查看对应的查看页面，其他地方与相关权限有关。

2、可以通过搜索功能搜索评论。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409385](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

评论搜索功能是对评论进行搜索，评论的回复和对评论的评论不进行搜索。

**三、注意事项**

 1、回复信息只在显示布局中显示，有权限查看模块数据的人员可以查看回复信息参与回复评论。

2、提交的评论在10分钟内允许修改、删除，超过10分钟不能修改、不能删除。

3、附加功能中引用的文档、附件、客户可以在回复也点击链接查看，但是只能查看信息页面，附件、文档的附件等信息的权限与文档本身的权限有关。

4、回复评论基础模块的布局是第一次开启回复评论功能的时候初始化生成的，

5、回复评论模块引用的表单不允许修改为其他表单，屏蔽选择表单按钮。

6、评论搜索功能只针对评论进行搜索，对评论的回复等信息不会进行搜索。

### 11.5.4、一人多岗（表单建模） {#11-5-4}

**一、概述**

1、可以设置数据是否统一在主账号显示。

2、开启数据统一在主账号显示时，主账号登录时，在查询列表，门户元素（建模自定义查询）中可以统一查看主次账号有权限的数据。

3、开启数据统一在主账号显示时，主账号登录时，浏览框选择数据时可以选择主次账号有权限的数据。

4、通过主账号操作主账号没有权限次账号有权限的数据时，日志中记录次账号信息。

5、主账号登录时，模块权限会取主账号和次账号最大权限，包括（查看、编辑、完全控制、模块监控权限）。

**二、功能说明**

1、有多个账号的人员通过主账号登录后，在个性化设置-其他设置中，设置多账号数据显示为统一在主账号显示。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409409](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2、设置后，查询列表中会统一显示主次账号有权限的数据，不需要进行切换。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409410](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

3、门户元素中会统一显示主次账号有权限的数据。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409411](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

4、浏览框选择数据时，会显示主次账号有权限的数据。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409413](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

5、主账号操作次账号有权限主账号没有权限的数据时，日志中会记录次账号的信息。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409416](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

6、主账号权限小于次账号时，主账号登录时，会取主账号和次账号的最大权限：

1）主账号权限小于次账号时，会取最大权限，如主账号是查看，次账号是完全控制，则主账号访问时有完全控制权限。

2）监控列表中，主账号只能访问监控列表菜单，但是没有模块监控权限，次账号有模块监控权限时，主账号在监控列表中也可以操作删除。

**三、注意事项**

1、主账号登录时，模块权限会取主次账号的最大权限，但是日志记录的时候是以有权限的记录，如主账号有查看权限没有编辑权限，次账号有编辑权限，则主账号查看时，日志记录主账号，编辑是记录次账号。

2、新建、查询、报表、监控菜单的权限还是独立根据权限控制。

3、树形数据显示时不受权限控制，但是点击链接打开模块数据时，取主次账号最大权限。

4、监控列表数据显示不受权限控制，监控列表删除数据时取主次账号模块中监控权限最大权限。

### 11.5.5、明细表数据过滤和排序功能 {#11-5-5}

**一、概述**

明细表数据可以根据某个特定的条件进行过滤 并且用户可以根据明细表中的某列排序来展现数据。

**二、应用场景说明**

例如有个项目任务的卡片 任务表为明细表 需要实现不同的任务负责人看到不同的明细表数据 并且用户可以根据明细表某列对明细表的数据进行排序

**三、功能说明**

**A、明细表数据过滤**

在【后端应用中心】-【表单引擎】-”某个具体的模块下的显示布局”如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1203478](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图1）

在显示布局上 当表单字段选择明细表的时候 在显示样式下 显示个“查询条件”字样 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1203480](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图2）

点击（图2）中的 “查询条件”弹出的页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1203482](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图3）

在（图3）上的设置 查询条件 如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1203483](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图4）

在设置（图4）那样的查询条件之后 显示的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1204423](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1、 明细表查询条可以设置sql条件和java条件 其中都支持解析动态参数。支持的动态参数如下

*   当前操作者 $UserId$
*   当前操作者部门$DepartmentId$
*   当前操作者部门（包含下级部门）$AllDepartmentId$
*   当前操作者分部$SubcompanyId$
*   当前操作者分部（包含下级分部）$AllSubcompanyId$
*   当前日期$date$

2、 明细表查询条件功能 是跟布局关联，不同的布局可以设置不同的明细表查询条件。

3、 同一个布局上可以针对不同的明细表设置不同的查询条件。

4、 编辑类型和显示类型的布局上都支持此功能。

**B、明细表数据排序**

在【后端应用中心】-【表单引擎】-”某个具体的模块下的显示布局”如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1203484](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                           （图5）

在（图5）的选择某个明细表中的某个字段 会显示出是否排序  如果勾选了则表示 此列在前端用户可以排序 如果不勾选则表示前端不排序

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1204420](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                        （图6）

在（图6）设置之后的前台显示的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1204421](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1、  明细表排序功能 是跟布局关联，不同的布局可以设置不同的明细表字段是否排序

2、  同一个布局上可以针对不同的明细表以及不同的明细表字段设置不同的排序。

3、  编辑类型和显示类型的布局上都支持此功能。

### 11.5.6、门户元素 {#11-5-6}

**一、概述**

通过门户元素功能，可以在门户设置元素时，通过建模自定义查询将表单建模中的查询列表添加到门户元素中，然后在门户中显示表单建模中配置的查询列表，将列表中的数据在门户中展示。

**二、应用场景说明**

当需要将建模中设置的查询列表在门户中显示时，可以通过在门户中添加建模自定义查询元素，将要展示在门户中的查询列表显示在门户中。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1096979](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、功能说明**

1、通过在【后端应用中心】→【门户引擎】→【门户页面】→【登录后页面】在对应的门户页面中设置元素。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1096982](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2、在设置元素页面，可以添加“建模自定义查询”元素，然后进行相应的设置，就可以将建模相关的查询列表显示在门户页面中。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1096986](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）通过点击建模自定义查询元素添加，通过设置图标进入建模自定义查询元素设置。

2）元素标题：设置元素的标题。

3）显示条数：设置列表显示条数。

4）链接方式：设置在门户元素列表中点击链接时，加载页面的方式。

当前页：在当前页面加载链接的页面。

弹出页：在弹出窗口中加载链接的页面。

5）列表：会加载通过在表单引擎中创建的查询列表，可以选择需要显示的查询列表。

6）字段：左侧会加载对应查询列表设置了显示标题的字段，然后可以选择要显示的在门户元素列表中的字段。通过在左侧双击选择要显示，右侧双击删除要显示的字段，也可以通过左右箭头选择从显示或者不显示的字段；通过上下箭头设置字段显示的顺序。

7）more：通过点击more链接到建模引擎中的查询列表页面。

8）刷新图标：点击可以刷新当前元素的数据列表。

3、设置后，建模自定义查询元素在门户中显示效果如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1096988](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**四、实施注意**

1、样式与共享功能与门户其他元素一致。

2、门户元素中显示的数据以及是否能显示列表与建模引擎中设置的模块权限和查询列表权限有关。

3、有维护者权限的人员才可以设置元素。

4、修改门户页面设置后，需要操作同步首页后才会刷新门户元素信息。

5、选择列表后，标题中只会显示查询列表设置为显示标题的字段。

6、门户元素中只会显示少量几条数据，需要查看更多数据，还需要通过点击more在查询列表中查看。

7、门户元素可以显示虚拟表单配置的列表数据。

8、门户元素可以显示主从表配置的列表数据。

### 11.5.7、建模分权 {#11-5-7}

**一、概述**

通过表单建模的分权管理，则可以实现分配机构权限给相应的管理员，则对应的管理员只能操作有权限的分部对应的表单建模相关数据，实现建模的分权管理。

**二、应用场景说明**

当需要指定分部管理员单独管理负责分部的建模数据时，可以通过表单建模分权管理来实现。

例如，A分部的管理员，只需要管理A分部的建模数据，则通过在角色设置中分配A分部的机构权限给A分部的管理员，那么A分部的管理员进入建模引擎时，则只可以操作A分部的建模数据。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343433](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、功能说明**

表单分权管理通过如下方式来设置：

1、开启建模分权

进入【后端应用中心】→【组织权限中心】→【权限管理】→【分权管理设置】，在【管理分权设置】中开启表单管理分权，同时总开关是否启用管理分权也会开启，设置默认机构后保存。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343435](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2、角色设置

1）为了方便后面角色设置中添加建模相关功能权限，可以通过进入【后端应用中心】→【组织权限中心】→【权限管理】→【权限设置】，新增权限组，将建模相关权限添加到权限组中。如下图（可选）。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343436](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2）进入【后端应用中心】→【组织权限中心】→【权限管理】→【角色设置】，新建赋权角色。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343437](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

3）在角色设置中，添加功能权限。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343456](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)4）在角色设置中，设置机构权限。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343458](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

权限说明：

禁止：与不勾选机构一致。

只读：所有相关页面为只读，不可编辑。

编辑：可新增、编辑，不可删除。

完全控制：可新增、编辑、删除。

5）在角色设置中，添加成员。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343459](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

3、进入表单建模

角色设置完成后，通过对应的人员登录系统进入建模引擎。

1）进入【后端应用中心】→【建模引擎】，切换分部后（如图1），会显示所选分部对应的数据（如图2）。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343465](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

图1

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343467](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

图2

2）新建或者编辑应用、模块、表单时，会默认显示所选择的分部，也可以修改为有权限选择的分部。应用：

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343469](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)模块：

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343470](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

表单：

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343471](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

3）建模相关页面，会根据设置的机构权限类型（只读、编辑、完全控制）显示。无权限：

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343472](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)只读：只读，不可编辑、不可删除，无保存按钮。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343474](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

编辑：可编辑、新增。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343475](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

完全控制：可新增、编辑、删除。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1343476](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**四、实施注意**

1、针对应用树，如果下级是有权限的，但是上级没有权限，则会显示上一级内容，但是没有权限操作。

2、查询、报表、浏览框、树、自定义页面、提醒没有单独分权，权限与应用一致。

3、模块、表单与所属应用关系，如果应用没有权限，但是模块或表单有权限，会显示对应的应用，但是应用没有操作权限。

4、应用、模块、表单的所属分部信息会根据如下规则生成：

1）建模分权开启时，根据选择的分部赋值。

2）为开启建模分权，分权总开关开启或者分权总开关存在默认值时，以分权总开关的值为准。

3）建模分权和分权总开关都不存在值时，取最小分部的id值。

5、前端查询列表的批量导入：

1）当有后端建模权限或者模块的批量导入权限时，相应的用户进入列表会显示批量导入按钮。

2）后端建模有批量导入的编辑或者完全控制权限，或者模块权限中设置了批量导入权限时，批量导入页面为可以编辑，可以正常导入；如果只有只读权限，则页面为只读，不可导入。