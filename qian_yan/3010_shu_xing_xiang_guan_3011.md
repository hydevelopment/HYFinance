## 【树形相关】

### 11.4.1复制树形 {#11-4-1}

**一、概述**

为表单建模后端树提供复制树功能，当需要新增类似的树时，则可以通过复制树功能来实现，复制树时可以将树和树节点设置信息都复制。

**二、功能说明**

1、通过进入【后端应用中心】→【建模引擎】→【树】，选择需要复制的树，在树信息页面或者树列表中操作右键复制树。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407319](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2、复制树后，会根据选择的树复制一个设置相同的树，新复制的树的名称为“原来树的名称-复制”。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407333](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、注意事项**

1、导航树、树形浏览框都支持复制树功能。

2、复制生成的树，设置与被复制的树相同。

### 11.4.2树形根节点主键值及treesqlwhere参数 {#11-4-2-treesqlwhere}

**一、概述**

为了更灵活的展示树节点数据，可以通过设置根节点主键值、是否显示根节点、treesqlwhere参数、链接地址json字符，设置树根据不同的设置进行数据展示。

**根节点主键值：**通过根节点主键值设置可以设置根节点要显示的内容。

**是否显示根节点：**可以设置树多级显示时，设置是否要显示根节点。

**treesqlwhere参数：**可以通过在链接目标中些treesqlwhere参数，使链接目标为模块查询列表时，根据设置的条件多条件查询。

**链接地址jason代码：**可以通过在链接地址中写一段json代码，树节点的链接目标则可以根据不同的条件加载到不同的地址。

**二、功能说明**

**A、根节点主键值**

通过在树节点设置中，通过在根节点主键值中输入固定值或者动态参数，设置当前树节点根据根节点主键显示相应的内容。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407591](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

1）通过设置指定主键值。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407594](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

2）通过设置动态参数，可以根据当前登录人员的UserId，DepartmentId，SubcompanyId进行过滤。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407598](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**B、是否显示根节点**

通过设置是否根节点选项，可以设置是否要显示根节点的内容，勾选显示，不勾选时，则不显示根节点的信息。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407607](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**C、treesqlwhere参数**

通过在链接目标中设置treesqlwhere参数，可以设置动态条件，树节点在加载数据时按照treesqlwhere条件进行显示，并且可以设置动态取当前表单的字段内容。如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407610](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：

treesqlwhere参数设置格式：url后面加：&amp;treesqlwhere=查询列表对应的表单中的字段名=固定值或者当前树节点对应表单的字段名and条件2…

示例：/formmode/search/CustomSearchBySimple.jsp?customid=441&amp;treesqlwhere=tslb=$id$and sm=&#039;图书001&#039;

**D、连接地址json字符**

通过链接地址json字符，可以通过在树节点的链接目标设置一段json代码，设置满足不同的条件，链接到不同的地址。

1、树节点json代码设置，如下图。

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407611](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

说明：jason条件设置格式如下：

1）格式：[{id:0,url:”地址1”},{id:2,url:”地址2”,sqlwhere:”sql条件”}]

2）其中id，url，sqlwhere为必填项。其中id只是个标识并不是树节点的id。

3）id为0表示为不满足其他条件时的默认地址，此项可以不输入sqlwhere。

示例：

[{id:0,url:&quot;http://www.weaver.com.cn&quot;},{id:1,url:&quot;/formmode/search/CustomSearchBySimple.jsp?customid=441&amp;treesqlwhere=tslb=$id$&quot;,sqlwhere:&quot;id in(2,3)&quot;}]

1、效果如下：

不符合条件的链接到设置的默认地址：

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407614](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

符合条件时，链接到对应的地址：

![E:\重要文件备份\ecology正式系统知识树图片(余海群提供)\20042\images\1407615](../assets/ezhong_yao_wen_jian_bei_4efd5c_ecology_zheng_shi_xi_tong_zhi_shi_shu_tu_724728_yu_hai_qun_ti_4f9b295c_2.png)

**三、注意事项**

1、根节点主键值支持设置固定值或者动态参数，固定值只支持整数，动态参数只支持UserId，DepartmentId，SubcompanyId。

2、treesqlwhere参数支持固定值或者动态参数值，需注意格式。

3、treesqlwhere参数试用需链接目标是查询列表地址的情况。

4、json字符支持固定值或者动态参数值，需注意格式。

5、json字符设置条件时，url代码可以设置系统内地址或者系统外地址，系统外地址需要加http://。