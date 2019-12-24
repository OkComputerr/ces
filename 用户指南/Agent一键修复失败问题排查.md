# Agent一键修复失败问题排查<a name="ces_01_0006"></a>

## 问题现象<a name="section19496021145519"></a>

安装主机监控Agent后，单击“修复插件配置”后，插件状态仍然是“配置异常”。

## 问题分析<a name="section2512759411"></a>

一键式修复插件失败后的排查思路：

1.  检查DNS配置。
2.  检查IAM委托配额。
3.  查看用户权限。

## 解决方法<a name="section103719241036"></a>

1.  检查DNS配置是否正确。
    1.  登录管理控制台。
    2.  单击“计算 \> 弹性云服务器”。
    3.  单击弹性云服务器名称。

        进入弹性云服务器详情页面。

    4.  单击基本信息中的虚拟私有云名称。

        进入虚拟私有云页面。

    5.  在虚拟私有云列表中，单击VPC名称链接。
    6.  在“子网”页签中查看弹性云服务器的DNS服务器地址是否正确。

        各区域DNS服务器地址配置以及如何修改DNS，请参考：[Windows](https://support.huaweicloud.com/usermanual-ces/zh-cn_topic_0150366044.html)和[Linux](https://support.huaweicloud.com/usermanual-ces/zh-cn_topic_0150354069.html)。

        ![](figures/zh-cn_image_0199251722.png)

2.  检查IAM委托配额。
    1.  登录管理控制台。
    2.  单击账户名下的“统一身份认证”。
    3.  在左侧导航树选择“委托”。
    4.  查看委托配额。

        查看是否有CESAgentAutoConfigAgency的委托。

        如果没有且配额已满，请删除不需要的配额后再次进行Agent一键修复。

        ![](figures/zh-cn_image_0199286165.png)

3.  检查用户权限。
    1.  登录管理控制台。
    2.  单击账户名下的“统一身份认证”。
    3.  在左侧导航树选择“用户组”。
    4.  单击账号所属用户组“操作”列下的“权限配置”。
    5.  Agent安装需要有以下权限：

        -   全局：Security Administrator
        -   Region：ECS User或BMS User以及CES Administrator或CES Admin权限

        ![](figures/zh-cn_image_0199275173.png)



