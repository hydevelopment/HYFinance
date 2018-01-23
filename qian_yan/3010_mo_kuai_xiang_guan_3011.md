## 【模块相关】

### 11.1.1、明细导入 {#11-1-1}

**一、概述**

明细导入是指存在明细表时，用户在新建卡片数据时，可以导入明细数据。

**二、应用场景说明**

例如一个客户卡片包含客户信息和联系人记录，其中联系人记录为明细表信息，当用户新建一个客户卡片时，可以通过明细导入功能导入多条联系人记录。

**三、功能说明**

1、后台配置：通过在模块中勾选“允许创建时导入明细”。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\5397](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2、前台应用：通过普通用户，在新建卡片数据时，通过明细导入操作可以导入明细数据。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\5371](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）下载模板：可以下载明细模板，可以在下载的明细模板中填写需要导入的明细数据。

2）上传Excel：可以通过上传Excel将填写了要导入的明细数据的模板上传后进行导入。

3）明细导入：上传Excel后，通过操作右键菜单中的明细导入可以将明细数据导入到当前卡片中。

**四、实施注意**

1、导入模板需注意：

1）导入明细数据时，会将原有明细内容删除，导入新的模板中的内容。

2）只有可编辑的字段才能进行导入，如果查看的字段有默认值的会自动加上默认值。

3）模板中第一行为表单明细字段名称，从第二行开始导入明细数据。

4）明细数据之间不能有空行。

5）如果有多个明细时模板中会有多个SHEET，一个明细一个SHEET.

6）数字类型字段不要有特殊格式，例如：科学计数法，千分位，货币符号等。

7）浏览类型字段直接输入名称，例如：人力资源字段直接输入人员名称。

8）check类型字段输入“1/0”或“是/否”。

9）下拉选择框类型字段输入下拉选择框显示名称。

2、需要在【后端应用中心】→【建模引擎】→【模块】对应模块中设置【允许创建时导入明细】功能时，前台创建卡片数据时才能操作明细导入。

3、操作明细导入时，会提示“数据还未保存，现在保存吗？”，需要点击【确定】后先保存数据再次操作【明细导入】。

### 11.1.2、模块导入导出 {#11-1-2}

**一、概述**

通过模块的导入导出，可以将模块及模块相关配置导入到zip数据文件中，然后通过模块导入的功能导入模块，生成模块相关配置信息，实现模块的快速添加配置。

**二、应用场景说明**

当不同的模块配置相同，或者需要将一个系统的模块相关信息添加到另外一个系统时，则可以通过模块的导入导出功能导出模块信息，再导入到要添加模块的系统中。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1094718](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、功能说明**

1、通过在【后端应用中心】→【建模引擎】→【模块】对应模块的基础页面操作导出模块，导出zip数据文件。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1094719](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）通过导出模块，保存的数据文件为zip格式。

2）导出模块后，会将模块相关的模块配置、对应表单、查询、报表、浏览框信息导出。

2、在【后端应用中心】→【建模引擎】→【应用】在需要导入模块的应用基本信息模块导入区域导入通过导出模块导出的文件。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1094720](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）通过模块导入可以导入通过导出模块生成的zip数据文件。

2）导入成功后，会将模块及模块对应的配置信息、表单、查询、报表、浏览框相关信息也导入。

3）支持实际表单和虚拟表单相关的模块。

4）如果导入的是虚拟表单，导入模块对应的系统中如果不存在的数据源也会导入，如果存在则不导入。

5）浏览框对应的浏览框列表中的标识也会导入，但是如果导入系统中存在相同的标识，则不导入。

6）导入模块对应的表单如果是自定义命名的表单如果系统中不存在相同表名的表单，新建的表单表名会也是自定义的，如果系统中已经存在相同表名的表单，则会按照（formtable_main_序列号）格式按照系统中序列号数字最大的加1生成表名，如formtable_main_1060。

3、导入成功后则会在操作导入的应用下新建导入的模块，以及模块相关的配置、表单、查询、报表、浏览框相关信息，但是布局和权限相关有关联的部分功能还需要重新设置。

**四、实施注意**

1、导入模块会导入模块配置、表单、查询、报表、浏览框相关信息，因为树、自定义页面等与模块没有关联关系，不作导入。

2、导入模块时，对应的自定义表单表名存在时，则会按照指定格式自动生成。

3、导入虚拟表单对应的模块时，如果对应的数据源导入系统存在则不作导入。

4、浏览框对应的浏览框标识，因为需要保持唯一性，如果系统中存在也不作导入。

5、模块导入是新增模块以及对应信息，重复导入会重复生成。

6、模块接口相关的配置因为存在关联性，不作导入。

7、上传目录、人员相关都是通过id进行查找，如果两个系统不一致，可能导入后会显示内容会不一致，需要重新设置。

8、导入完成后，针对浏览框的链接目标信息可能不准确，最好通过浏览框标识的初始化功能重新初始化一下。

### 11.1.3、应用导入导出 {#11-1-3}

**一、概述**

通过应用的导入导出可以一次性将应用及应用下的模块、表单、查询、报表、浏览框、树、自定义页面等信息导入到系统中，实现应用的快速添加。

**二、应用场景说明**

如需要从一个系统将整个应用及应用下的信息迁移到了另外一个系统中时，则可以通过应用的导入导出功能导入相关信息后再稍做配置就可以快速完成一个应用的配置了。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1094730](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、功能说明**

1、通过在【后端应用中心】→【建模引擎】→【应用】在对应的应用信息页面通过右键导出应用或者通过在左侧应用树点击要导出的应用操作导出应用。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1094733](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：导出应用后保存为zip文件，以供导入使用。

2、通过导入应用导入通过导出应用导出的文件，导入完成后会在操作导入应用下级新增导入的应用。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1094734](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）导入应用时，只能导入通过导出应用导出的文件。

2）导入应用后，会导入当前应用下的模块、表单、查询、报表、浏览框、树、自定义页面等相关信息，不支持下级应用的导入。

3）导入应用功能是新增应用，重复导入会重复新增。

4）导入应用后，权限、页面扩展、树存在关联性的功能可能不能成功导入，需要重新设置。

5）浏览框标识、数据源等系统中存在相同内容时，不作导入。

6）自定义表单如果存在相同表名的表单，则会按照（formtable_main_序列号）的格式自动生成。

**四、实施注意**

1、应用导入成功后，需要手动刷新页面重新加载应用树才能显示导入的应用。

2、导入应用是在系统中实现新增应用，重复导入会重复新增。

3、浏览框标识、数据源等系统中存在相同内容时，不作导入。

4、自定义表单表名如果系统中存在时，则会按照规定的格式自动生成表名。

5、外部接口配置、页面扩展以及树中链接目标相关功能存在关联性，不作导入，应用导入后需要重新配置。

6、应用导入不支持下级应用的导入。

7、导入完成后，针对浏览框的链接目标信息可能不准确，最好通过浏览框标识的初始化功能重新初始化一下。

### 11.1.4、受限制字段控制角色权限 {#11-1-4}

**一、概述**

在后台权限规则中，添加共享类型为角色的权限，设置限制条件，满足条件的角色成员有模块权限

**二、应用场景说明**

当需要共享卡片数据权限给跟创建人属于同一个部门的角色成员,可以在后台添加角色共享规则。在前台新建数据，满足跟创建人属于同一个部门的角色成员才权限查看该条数据（如下图）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1278951](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、功能说明**

1，在[后台设置]-[模块]-[权限]中添加默认共享，共享类型选择“角色”，角色是否受范围限制选择“是”

说明：

1）字段类型选择“人员”如下图，共享级别有“部门、分部、总部”，选择共享级别和限制字段后保存规则。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1278968](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

如果共享级别选择部门，角色人员满足跟限制字段内容中人员是同一个部门，具有模块共享权限

如果共享级别选择分部，角色人员满足跟限制字段内容中人员是同一个分部，具有模块共享权限

如果共享级别选择总部，角色人员满足跟限制字段内容中人员是同一个总部，具有模块共享权限

2）字段类型选择“部门”如下图，没有共享级别设置，选择限制字段后添加规则保存，角色中的人员满足属于限制字段内容中部门，具有模块共享权限

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1278960](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

3）字段类型选择“分部”如下图，没有共享级别设置，选择限制字段后添加规则保存，角色中的人员满足属于限制字段内容中分部，具有模块共享权限

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1278963](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**四、实施注意**

1，前台添加共享或者批量共享，支持此功能,

2，系统管理员不在组织架构中，设置的限制字段内容是sysadmin时，规则解析不出来，不支持此功能设置 

3，在前台显示页面右键共享，添加角色权限，如果角色成员都不满足此条件，添加时会提示：“按照你的限制条件，在角色中没有满足条件的人员”

4，角色是否受权限选择是时，会根据角色范围限制解析出人员，在角色中添加、或者删除人员后需要操作权限重构

### 11.1.5、权限规则条件 {#11-1-5}

**一、概述**

此功能用于在表单建模后台模块中的权限设置用于满足一定条件之后权限才会生效。

1、目前权限规则条件只用于默认共享（创建人相关），默认共享两块设置的权限规则。

2、默认共享（创建人相关）需要设置了某种权限类型右键保存之后才会出现条件。

目前权限规则条件功能设置条件有两种方式

第一种界面化的形式设置（普通类型），第二种通过写sql的方式（sql）。 

**二、应用场景说明**

后台表单引擎中的模块关联的权限需要支持条件。所谓的支持条件就是满足了特定的条件之后此权限规则才会生效。

应用场景如下：

模块关联表单 表单中比如有个类型的下拉框字段对应的值为A，B 我的需求是当类型字段的值为A的时候我需要test1这个人来看 当类型字段值为B的时候我需要test2才可以看。

针对以上需求 我们就可以使用权限规则条件这个功能来实现。Test1,test2分别建2条权限规则然后在这2条规则上设置条件test1的条件是 类型的值=A，test2的条件是类型的值=B。这样就可以实现当前端数据类型的值=A的时候 test1这个人可以有权限查看，当前端数据类型的值=B的时候 test2这个人可以有权限查看这条数据。

综上所述的应用场景表单建模权限规则条件支持所有类型字段设置条件并且支持各种字段组合设置。也支持明细表中的字段设置条件及各种类型的字段组合设置的条件。

**三、功能说明**

在【后端应用中心】----【建模引擎】---“某个具体的模块”---“权限”在此tab页上设置的权限规则后面可以添加条件如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330851](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图1）

**3.1.界面化的形式设置条件（普通类型）**

一、接下来介绍权限规则条件的第一种方式：界面化的形式设置条件（普通类型）

A、点击（图1）中的权限规则后条件后的![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330852](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)弹出的页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330858](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图2）

B、在（图2）的页面上我们选择目标字段操作类型及相应的值然后点击添加按钮具体如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330881](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图3）

不同类型字段对应的操作类型及填写值的对应关系如下

| **字段** | **操作** | **值** |
| --- | --- | --- |
| 单行文本—文本 | 等于，不等于，包含，不包含 | 单行文本输入框 |
| 单行文本—整数 | 大于，大于或等于，小于，小于或等于，等于，不等于 | 单行文本输入框 |
| 单行文本—浮点数 | 大于，大于或等于，小于，小于或等于，等于，不等于 | 单行文本输入框 |
| 单行文本—金额转换 | 等于，不等于 | 单行文本输入框 |
| 单行文本—金额千分位 | 等于，不等于，包含，不包含 | 单行文本输入框 |
| 多行文本 | 等于，不等于，包含，不包含 | 多行文本输入框 |
| 浏览框—日期 | 大于，大于或等于，小于，小于或等于，等于，不等于 | 日期控件 |
| 浏览框—日期 | 大于，大于或等于，小于，小于或等于，等于，不等于 | 时间控件 |
| 浏览框 | 等于 | 浏览框控件 |
| 选择项 | 等于，不等于 | 下拉框控件 其中包含null |
| Check | 等于 | 下拉框控件 null,0,1 |

可以添加多个字段的组合条件具体如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330884](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图4）

添加完的条件可以双击再次编辑如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330886](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图5）

添加完的条件可以选择多条设置条件与条件之间的关系如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330887](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图6）

添加完的条件也可以选择条件进行删除如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330888](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图7）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330889](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图8）

C、设置完条件之后在我们的条件规则上显示如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330890](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图9）

D、以上步骤设置完成之后如果需要对老数据起作用的话必须右键点击“权限重构”按钮之后老数据才会生效如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330892](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图10）

E、以上步骤完之后肖荣娟查看权限设置的条件是文本包含test的那么肖荣娟查看这个模块的数据的时候只能看到文本包含test的数据效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330894](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图11）

**3.2.Sql****形式设置条件（sql）**

A、点击（图1）中的权限规则后条件后的![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330913](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)弹出的页面如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330895](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图12）

B、选择（图12）页面上的 sql 效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330900](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图13）

C、在（图13）上可以编写sql编写sql的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1330904](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图14）

D、以上设置完之后然后跟以上（界面化形式设置条件中的D步骤）一样需要右键权限重构之后老数据才会生效。

**四、实施注意**

1、此功能虚拟表单挂的模块设置的权限也支持此功能的生效是需要单独点开卡片的时候才会判断列表中的数据是不会判断的虚拟表单是默认所有人拥有查看权限的。

2、在权限上添加条件或者清空条件都需要点击“权限重构”按钮老数据才会生效。

3、默认共享（创建人相关）添加条件或者清空条件勾选后面的“更新表单数据”保存之后老数据也会生效。

### 11.1.6、单条权限规则历史数据重构 {#11-1-6}

**一、概述**

1、在此功能之前的配置的权限规则 不支持单条权限规则历史数据重构功能。只有当右键点击【模块】--【权限】页面上“权限重构”按钮之后所有规则重新生成权限数据之后才拥有此功能。

2、在更新此功能之后增加的权限规则就支持此功能 在新增的规则后面会出现个“权限重构”的字体点击这个链接会根据此条权限规则对历史数据进行权限重构。

**二、功能说明**

A、更新此功能之前设置的权限规则如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408922](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                                               （图1）

（图1）这个页面是在更新此功能之前增加的权限规则。我们可以在（图1）页面上右键点击“权限重构”按钮如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408925](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图2）

点击（图2）页面上的“权限重构”按钮之后老的权限规则也会显示“权限重构”字体链接如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408926](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图3）

在（图3）页面上我们可以点击“权限重构”这个链接对单条权限规则进行历史数据重构。

B、更新此功能代码之后新增的权限规则就会加上“权限重构”的链接如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408930](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                                     （图4）

（图4）页面上是新增的权限规则保存完规则之后后面会出现“权限重构”的链接点击此链接出来的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408936](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

 （图5）

点击（图5）页面上的“确定“按钮之后则针对这条权限规则进行历史数据权限重构。

### 11.1.7、批量导入类型增加权限控制及新增更新类型 {#11-1-7}

**一、概述**

1、批量导入权限控制导入类型 可以控制有批量导入权限的人 导入类型只有一种或者多种。

2、批量导入功能增加一种更新的导入类型实现根据某个关键字字段去更新系统已经存在的数据 如果能找到就更新 不能找到则插入

**二、功能说明**

**A、批量导入类型控制**

在【后端应用中心】----【表单引擎】---“某个具体的模块”---“权限”此tab页面上可以设置批量导入权限及导入类型如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408953](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                                    （图1）

点击（图1）中的“添加”弹出的页面如下图在此页面上可以设置批量导入权限及导入类型具体如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408959](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                                                        （图2）

在（图2）设置完的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408960](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                                                       （图3）

在图（3）中设置了肖1这个用户有批量导入的权限并且导入类型只有“追加”这种类型。现在我们以肖1这个用户登录系统然后在此模块对应的查询进行批量导入的时候我们的导入类型只能选择“追加”具体如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408962](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图4）

从（图4）中我们可以看出肖1这个人有批量导入权限并且导入类型只有“追加”从而达到了控制导入类型。

注意点：

1、老数据默认是全部类型（包括：追加，覆盖，更新）

2、如果此用户是系统管理员的话那么默认也是有全部类型的

3、如果系统管理角色中有此用户权限中批量导入也设置了此用户那么此用户的导入类型以权限设置的为主

**B、批量导入增加更新导入类型**

在批量导入类型的页面增加一种“更新”的导入类型此类型是用于导入excel的时候可以根据某个关键字字段对已经存在的数据进行更新。具体操作步骤如下图

1、在【后端应用中心】---【表单引擎】---“模块”具体的权限tab页设置导入权限并且设置导入类型操作如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408965](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图5）

在（图5）添加肖1有批量导入权限且导入类型为“更新”增加的权限如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408966](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图6）

在后端设置完权限此时用户登录系统前端看到的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408968](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图7）

此时我们的系统中已经有的数据然后我们系统把老数据的某个列值更新成excel中的内容如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408969](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图8）

要实现（图8）中的效果肖1 这个用户登录系统然后在此查询中右键点击“批量导入”按钮出现的效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408970](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图9）

在（图9）页面上上传excel然后重复验证字段选择文本导入类型选择更新具体效果如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408981](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图10）

点击（图10）页面上的“开始导入”按钮导入成功此是我们看下数据已经将老数据成功更新为excel中的值。如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408985](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

                   （图11）

我们系统中已经存在数据如果excel中值能找到则更新不能找到则直接插入针对这种情况的处理步骤只需要在批量导入的页面把“是否更新失败的数据选择追加”前的复选框勾选即可。如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408986](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

（图12）

注意点：

1、当导入类型选择更新时重复验证字段是必填的必须要根据重复验证字段去更新数据。

2、更新有2中情况一种是能找到的数据就直接更新不能找到的就导入失败，另外一种是能找到的就直接更新不能找到的直接插入。针对这2种情况是由“是否更新失败的数据选择追加”前的复选框来决定的（具体如（图12）中的说明）

在使用表单建模批量导入功能的总结：

1、明细表单字段不支持重复验证字段也就是说如果是主从表明细表的数据是一直追加的

2、自定义单选，自定义多选，树形单选，树形多选，虚拟表单单选，虚拟表单多选类型的字段都支持批量导入。

3、当导入类型为更新的时候就必须选择重复验证字段数据是根据选择的字段去更新值的。

4、关联的浏览框有重名的则会随机找一条导入进去。

5、导入类型为追加，覆盖，更新都可以支持字段重复验证。

### 11.1.8、默认共享（创建人相关）单条规则历史数据重构 {#11-1-8}

**一、概述**

通过默认共享（创建人相关）单条规则的历史数据重构功能，可以在修改默认共享（创建人相关）单条权限规则后，通过勾选更新表单数据，则针对单条规则，历史数据可以进行权限重构。

**二、功能说明**

通过进入【后端应用中心】→【建模引擎】→【模块】，进入对应的模块的权限页面。如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408996](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

勾选对应规则的更新表单数据，然后保存。如下图

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408998](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

针对创建人本人、创建人直接上级、创建人所有上级、创建人本分部、创建人本部门都可以操作更新表单数据。

针对历史数据，只有勾选了更新表单数据对应的规则会进行权限重构

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1408999](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、注意事项**

1、勾选规则对应的更新表单数据保存后，旧的权限会失效，新的权限生效。

2、修改了创建人上级、部门、分部信息后，需要更新表单数据后，新的上级，部门人员、分部人员才会有权限。 

### 11.1.9、建模权限支持所有上级解析 {#11-1-9}

**一、概述**

1、通过与创建人相关的默认共享中的创建人所有上级功能，可以设置创建人所有上级的权限。

2、通过模块主字段中设置人员的上级关系，可以设置模块人员字段相关人员的直接上级、所有上级的权限

**二、功能说明**

1、通过进入【后端应用中心】→【建模引擎】→【模块】，进入对应模块的权限tab页。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409018](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2、默认共享（创建人相关）可以设置创建人所有上级的相关权限，如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409023](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）设置创建人所有上级相关权限后，则会解析创建人的所有上级信息。

2）没有权限：创建人所有上级没有权限。

3）查看：创建人所有上级有查看权限，可以设置对应的查看布局。

4）编辑：创建人所有上级有编辑权限，可以设置对应的查看、编辑布局。

5）完全控制：创建人所有上级有完全控制权限，可以设置对应的查看、编辑布局。

3、默认共享中，可以设置模块主字段选择对应的人员字段可以设置人员的当前人员、直接上级、所有上级相关权限。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409074](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

1）共享类型选择模块主字段、字段类型为人员时，可以设置上级关系。

2）上级关系可以设置当前人员、人员直接上级、人员所有上级。

当前人员：选择当前人员时，只有模块字段中对应的人员有权限。

人员直接上级：选择人员直接上级时，模块字段中对应的人员的直接上级有相关权限。

人员所有上级：选择人员所有上级时，模块字段中对应的人员的所有上级有相关权限。

3）更新表单数据：保存权限时，勾选更新表单数据，则会根据当前添加的规则更新历史数据权限。

4）可以通过查看布局、编辑布局、布局级别设置权限对应的人员加载的布局，布局级别越小，优先级越高。

5）权限项：可以设置查看、编辑、完全控制权限。

4、权限设置完成之后，会根据创建人、模块字段解析相关的权限。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409077](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、实施注意**

1、当人员上级发生变化时，针对历史数据，需要权限重构后才会解析到新的上级。

2、当人员上级发生变化时，修改模块数据，会按照新的上级解析权限。

3、当设置的是多人员字段时，如果不同的人的所有上级中有相同的上级，则在共享对象中会显示多个相同的人员。

### 11.1.10、权限支持安全级别范围检索 {#11-1-10}

**一、概述**

1、添加模块权限，安全级别设置下限值，共享对象中安全级别大于该值的人员有权限查看数据

2、添加模块权限，安全级别设置下限值和上限值，共享对象中安全级别在上下限范围内的人员有权限查看数据

**二、功能说明**

添加模块权限，安全级别设置下限值，保存权限规则后（如图1），在前台新建表单数据保存，共享对象中满足大于安全级别设置下限值的人员才有查看数据权限，如图2

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409163](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

图1

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409164](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

图2

添加模块权限，安全级别设置下限值和上限值，保存权限规则后（如图3），在前台新建表单数据保存，共享对象中满足大于下限值、小于上限值的人员才有查看数据权限（如图4）

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409165](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

图3

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409167](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

图4

**三、实施注意**

 1、安全级别范围包括有:

a、所有人安全级别范围

b、部门，分部安全级别范围

c、角色安全级别范围

d、模块主字段人员，部门，分部安全级别范围

e、创建人相关的分部，部门所有上级等支持安全级范围取值

2、安全级别下限为必填项，默认值是10

3、支持引用虚拟表单生成的模块

### 11.1.11、单条规则删除及删除权限数据 {#11-1-11}

**一、概述**

为表单建模实现删除默认共享单条规则时，可以选择是否需要删除当前规则对应的数据权限。

**二、功能说明**

通过进入【后端应用中心】→【表单建模】→【模块】，选择对应的模块，进入权限tab页，点击需要删除的默认共享权限规则后的权限删除。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409172](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

弹出提示，确认是否要删除，点击确定删除，点击取消不删除。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409173](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

确定删除权限规则后，弹出提示是否删除此权限对应的数据权限，确定删除，取消不删除。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409176](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

如果选择删除权限对应数据权限，则模块历史数据对应的权限会被删除，不需要再操作权限重构。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1409178](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、注意事项**

1、默认共享中的权限都支持权限删除。

2、操作权限删除时只会删除当前规则对应的数据权限。

如果操作权限删除时，选择不删除当前权限对应的数据权限，则历史数据权限仍然存在，新建的数据则按照新的权限规则。