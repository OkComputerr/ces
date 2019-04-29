# 修改DNS与添加安全组<a name="ZH-CN_TOPIC_0150366044"></a>

## 操作场景<a name="zh-cn_topic_0078544024_section10035481163223"></a>

本章节指导用户为Linux系统的ECS或BMS主机添加域名解析并添加安全组，防止下载Agent安装包与采集监控数据时出现异常。

>![](public_sys-resources/icon-note.gif) **说明：**   
>添加DNS服务解析和配置安全组针对的是主网卡。  

## 操作步骤<a name="section1251913413419"></a>

1.  VNC方式登录Windows弹性云服务器。
2.  打开“控制面板 \> 网络与共享中心”，单击“更改适配器配置”。
3.  右键单击使用的网络，打开设置，按如下所示配置DNS。

    **图 1**  添加域名解析地址<a name="fig169461062266"></a>  
    ![](figures/添加域名解析地址-0.png "添加域名解析地址-0")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >不同区域nameserver不同，如下所示：  
    >华北-北京一：100.125.1.250,100.125.21.250  
    >华北-北京四：100.125.1.250,100.125.129.250  
    >华东-上海二：100.125.17.29,100.125.135.29  
    >华南-广州：100.125.1.250,100.125.136.29  
    >亚太-香港：100.125.1.250,100.125.3.250  
    >亚太-曼谷：100.125.1.250,100.125.3.250  

4.  在管理控制台修改子网DNS服务器地址。
    1.  在管理控制台左上角单击![](figures/icon-region.png)图标，选择区域和项目。
    2.  选择“服务列表 \> 计算 \> 弹性云服务器”。

        弹性云服务器列表中，单击ECS名称查看详情。

    3.  在“虚拟私有云”项单击“vpc-ces”，进入“虚拟私有云”界面。如[图2](#zh-cn_topic_0150354069_fig0772121318363)所示。

        **图 2**  虚拟私有云<a name="zh-cn_topic_0150354069_fig0772121318363"></a>  
        ![](figures/虚拟私有云.png "虚拟私有云")

    4.  在“VPC名称/ID”列表中，单击“vpc-ces”。
    5.  在“子网”列表中，单击“subnet-3e3b”所在行“修改”。

        弹出“修改子网”对话框，修改“DNS服务器地址1”为“100.125.1.250”。如[图3](#zh-cn_topic_0150354069_fig6241144284010)所示。

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >-   subnet-3e3b为该ECS的子网。  
        >-   DNS服务器地址与[2](修改DNS与添加安全组.md#zh-cn_topic_0078544024_li30189854165124)中的nameserver保持一致。  

        **图 3**  修改DNS服务器地址<a name="zh-cn_topic_0150354069_fig6241144284010"></a>  
        ![](figures/修改DNS服务器地址.png "修改DNS服务器地址")

    6.  单击“确定”，保存设置。

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >在控制台修改DNS需重启ECS或BMS后生效。  


5.  在管理控制台修改ECS使用的安全组规则。
    1.  在ECS详情页，单击安全组页签，进入安全组列表页。
    2.  单击具体的安全组名，单击“更改安全组规则”，进入安全组详情页。
    3.  在该安全组详情页，单击“出方向规则 \> 添加规则 ”，按[表1](#zh-cn_topic_0150354069_table89472534275)所示添加规则。

        **表 1**  安全组规则

        <a name="zh-cn_topic_0150354069_table89472534275"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0150354069_row12943453152710"><th class="cellrowborder" valign="top" width="11%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0150354069_p69421453152713"><a name="zh-cn_topic_0150354069_p69421453152713"></a><a name="zh-cn_topic_0150354069_p69421453152713"></a>方向</p>
        </th>
        <th class="cellrowborder" valign="top" width="11.43%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0150354069_p149428533277"><a name="zh-cn_topic_0150354069_p149428533277"></a><a name="zh-cn_topic_0150354069_p149428533277"></a>协议</p>
        </th>
        <th class="cellrowborder" valign="top" width="8.21%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0150354069_p69424532275"><a name="zh-cn_topic_0150354069_p69424532275"></a><a name="zh-cn_topic_0150354069_p69424532275"></a>端口</p>
        </th>
        <th class="cellrowborder" valign="top" width="69.36%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0150354069_p894395312278"><a name="zh-cn_topic_0150354069_p894395312278"></a><a name="zh-cn_topic_0150354069_p894395312278"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0150354069_row49431153112718"><td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0150354069_p1494312539277"><a name="zh-cn_topic_0150354069_p1494312539277"></a><a name="zh-cn_topic_0150354069_p1494312539277"></a>出方向</p>
        </td>
        <td class="cellrowborder" valign="top" width="11.43%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0150354069_p14943185382715"><a name="zh-cn_topic_0150354069_p14943185382715"></a><a name="zh-cn_topic_0150354069_p14943185382715"></a>TCP</p>
        </td>
        <td class="cellrowborder" valign="top" width="8.21%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0150354069_p594325317274"><a name="zh-cn_topic_0150354069_p594325317274"></a><a name="zh-cn_topic_0150354069_p594325317274"></a>80</p>
        </td>
        <td class="cellrowborder" valign="top" width="69.36%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0150354069_p16651028185814"><a name="zh-cn_topic_0150354069_p16651028185814"></a><a name="zh-cn_topic_0150354069_p16651028185814"></a>用于从OBS桶下载Agent包到ECS或BMS中、获取ECS或BMS的元数据信息与鉴权信息。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0150354069_row6944145315277"><td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0150354069_p69441453102716"><a name="zh-cn_topic_0150354069_p69441453102716"></a><a name="zh-cn_topic_0150354069_p69441453102716"></a>出方向</p>
        </td>
        <td class="cellrowborder" valign="top" width="11.43%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0150354069_p1394425315273"><a name="zh-cn_topic_0150354069_p1394425315273"></a><a name="zh-cn_topic_0150354069_p1394425315273"></a>TCP、UDP</p>
        </td>
        <td class="cellrowborder" valign="top" width="8.21%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0150354069_p6944185312278"><a name="zh-cn_topic_0150354069_p6944185312278"></a><a name="zh-cn_topic_0150354069_p6944185312278"></a>53</p>
        </td>
        <td class="cellrowborder" valign="top" width="69.36%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0150354069_p1051336115813"><a name="zh-cn_topic_0150354069_p1051336115813"></a><a name="zh-cn_topic_0150354069_p1051336115813"></a>用于DNS解析域名，下载Agent时解析OBS地址、发送监控数据时解析云监控服务Endpoint地址。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0150354069_row19947105314275"><td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0150354069_p1894418532279"><a name="zh-cn_topic_0150354069_p1894418532279"></a><a name="zh-cn_topic_0150354069_p1894418532279"></a>出方向</p>
        </td>
        <td class="cellrowborder" valign="top" width="11.43%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0150354069_p15947145313278"><a name="zh-cn_topic_0150354069_p15947145313278"></a><a name="zh-cn_topic_0150354069_p15947145313278"></a>TCP</p>
        </td>
        <td class="cellrowborder" valign="top" width="8.21%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0150354069_p1194755318274"><a name="zh-cn_topic_0150354069_p1194755318274"></a><a name="zh-cn_topic_0150354069_p1194755318274"></a>443</p>
        </td>
        <td class="cellrowborder" valign="top" width="69.36%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0150354069_p2748650125812"><a name="zh-cn_topic_0150354069_p2748650125812"></a><a name="zh-cn_topic_0150354069_p2748650125812"></a>采集监控数据到云监控服务端。</p>
        </td>
        </tr>
        </tbody>
        </table>



