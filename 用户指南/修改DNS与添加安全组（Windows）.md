# 修改DNS与添加安全组（Windows）<a name="ZH-CN_TOPIC_0150366044"></a>

## 操作场景<a name="zh-cn_topic_0078544024_section10035481163223"></a>

本章节指导用户为Windows系统的ECS主机添加域名解析并添加安全组，防止下载Agent安装包与采集监控数据时出现异常。

>![](public_sys-resources/icon-note.gif) **说明：**   
>添加DNS服务解析和配置安全组针对的是主网卡。  

## 修改DNS（Windows图形化界面）<a name="section1251913413419"></a>

修改ECS的DNS配置有两种方式：Windows图形化界面和管理控制台。您可以根据自己的使用习惯选择其中一种方式进行配置。

本节介绍使用Windows图形化界面方式添加域名解析地址至resolv.conf文件的操作步骤和方法。

如果想要使用管理控制台方式，请参考[修改DNS（管理控制台方式）](#section17618113213119)。

1.  VNC方式登录Windows弹性云服务器。
2.  打开“控制面板 \> 网络与共享中心”，单击“更改适配器配置”。
3.  右键单击使用的网络，打开设置，配置DNS。

    **图 1**  添加域名解析地址（Windows）<a name="fig169461062266"></a>  
    ![](figures/添加域名解析地址（Windows）.png "添加域名解析地址（Windows）")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >不同区域nameserver不同，如下所示：  
    >华北-北京一：100.125.1.250,100.125.21.250  
    >华北-北京四：100.125.1.250,100.125.129.250  
    >华东-上海二：100.125.17.29,100.125.135.29  
    >华南-广州：100.125.1.250,100.125.136.29  
    >亚太-香港：100.125.1.250,100.125.3.250  
    >亚太-曼谷：100.125.1.250,100.125.3.250  
    >亚太-新加坡：100.125.1.250  
    >非洲-约翰内斯堡：100.125.1.250  
    >华东-上海一：100.125.1.250,100.125.64.250  


## 修改DNS（管理控制台方式）<a name="section17618113213119"></a>

本节介绍登录管理控制台后修改ECS的DNS配置的操作步骤和方法。本章节以ECS为例介绍如何修改DNS和添加安全组，BMS操作步骤类似。

1.  在管理控制台左上角单击![](figures/icon-region-0.png)图标，选择区域和项目。
2.  选择“服务列表 \> 计算 \> 弹性云服务器”。

    弹性云服务器列表中，单击ECS名称查看详情。

3.  在“虚拟私有云”项单击“vpc-ces”，进入“虚拟私有云”界面。如[图2](#zh-cn_topic_0150354069_fig1939913311051)所示。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >此处假设 vpc-ces为当前ECS所使用的虚拟私有云。  

    **图 2**  虚拟私有云<a name="zh-cn_topic_0150354069_fig1939913311051"></a>  
    ![](figures/虚拟私有云.png "虚拟私有云")

4.  在“名称”列表中，单击“vpc-ces”。
5.  在“子网”列表中，单击“subnet-3e3b”所在行“修改”。

    弹出“修改子网”对话框，修改“DNS服务器地址1”为“100.125.1.250”和“100.125.21.250”。如[图3](#zh-cn_topic_0150354069_fig240020311758)所示。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >subnet-3e3b为该ECS的子网。  
    >DNS服务器地址与[3](修改DNS与添加安全组（Linux）.md#zh-cn_topic_0078544024_li30189854165124)中的nameserver保持一致。  

    **图 3**  修改DNS服务器地址<a name="zh-cn_topic_0150354069_fig240020311758"></a>  
    ![](figures/修改DNS服务器地址.png "修改DNS服务器地址")

6.  单击“确定”，保存设置。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >在控制台修改DNS需重启ECS或BMS后生效。  


## 修改ECS的安全组规则（管理控制台）<a name="section86832021101817"></a>

本节介绍登录管理控制台后修改ECS安全组规则的操作步骤和方法。本章节以ECS为例介绍如何修改DNS和添加安全组，BMS操作步骤类似。

1.  在ECS详情页，单击安全组页签。

    进入安全组列表页。

2.  单击具体的安全组名。
3.  单击“更改安全组规则”。

    进入安全组详情页。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >BMS的操作步骤：  
    >1.  请单击表格中左上角的安全组ID。  
    >2.  在对应安全组“操作”列单击“配置规则”。  

4.  在“出方向规则”页签下单击“添加规则”。
5.  按[表1](#zh-cn_topic_0150354069_table168311845185818)所示添加规则。

    **表 1**  安全组规则

    <a name="zh-cn_topic_0150354069_table168311845185818"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0150354069_row4830164565810"><th class="cellrowborder" valign="top" width="14.261426142614262%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0150354069_p1283074595819"><a name="zh-cn_topic_0150354069_p1283074595819"></a><a name="zh-cn_topic_0150354069_p1283074595819"></a>方向</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.831483148314831%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0150354069_p15830104525818"><a name="zh-cn_topic_0150354069_p15830104525818"></a><a name="zh-cn_topic_0150354069_p15830104525818"></a>协议</p>
    </th>
    <th class="cellrowborder" valign="top" width="11.781178117811782%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0150354069_p3830134510582"><a name="zh-cn_topic_0150354069_p3830134510582"></a><a name="zh-cn_topic_0150354069_p3830134510582"></a>端口</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.512151215121513%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0150354069_p1783013453580"><a name="zh-cn_topic_0150354069_p1783013453580"></a><a name="zh-cn_topic_0150354069_p1783013453580"></a>目的地址</p>
    </th>
    <th class="cellrowborder" valign="top" width="37.61376137613761%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0150354069_p5830845175811"><a name="zh-cn_topic_0150354069_p5830845175811"></a><a name="zh-cn_topic_0150354069_p5830845175811"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0150354069_row1983154575816"><td class="cellrowborder" valign="top" width="14.261426142614262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0150354069_p1883044555818"><a name="zh-cn_topic_0150354069_p1883044555818"></a><a name="zh-cn_topic_0150354069_p1883044555818"></a>出方向</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.831483148314831%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0150354069_p3830114525817"><a name="zh-cn_topic_0150354069_p3830114525817"></a><a name="zh-cn_topic_0150354069_p3830114525817"></a>TCP</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.781178117811782%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0150354069_p1983015458583"><a name="zh-cn_topic_0150354069_p1983015458583"></a><a name="zh-cn_topic_0150354069_p1983015458583"></a>80</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.512151215121513%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0150354069_p08301345155818"><a name="zh-cn_topic_0150354069_p08301345155818"></a><a name="zh-cn_topic_0150354069_p08301345155818"></a>100.125.0.0/16</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.61376137613761%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0150354069_p20830184517586"><a name="zh-cn_topic_0150354069_p20830184517586"></a><a name="zh-cn_topic_0150354069_p20830184517586"></a>用于从OBS桶下载Agent包到ECS或BMS中、获取ECS或BMS的元数据信息与鉴权信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0150354069_row2831194517589"><td class="cellrowborder" valign="top" width="14.261426142614262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0150354069_p6831174555814"><a name="zh-cn_topic_0150354069_p6831174555814"></a><a name="zh-cn_topic_0150354069_p6831174555814"></a>出方向</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.831483148314831%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0150354069_p68311145125811"><a name="zh-cn_topic_0150354069_p68311145125811"></a><a name="zh-cn_topic_0150354069_p68311145125811"></a>TCP、UDP</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.781178117811782%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0150354069_p1783124555811"><a name="zh-cn_topic_0150354069_p1783124555811"></a><a name="zh-cn_topic_0150354069_p1783124555811"></a>53</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.512151215121513%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0150354069_p188311455587"><a name="zh-cn_topic_0150354069_p188311455587"></a><a name="zh-cn_topic_0150354069_p188311455587"></a>100.125.0.0/16</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.61376137613761%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0150354069_p1383116456581"><a name="zh-cn_topic_0150354069_p1383116456581"></a><a name="zh-cn_topic_0150354069_p1383116456581"></a>用于DNS解析域名，下载Agent时解析OBS地址、发送监控数据时解析云监控服务Endpoint地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0150354069_row10831174512586"><td class="cellrowborder" valign="top" width="14.261426142614262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0150354069_p583194512587"><a name="zh-cn_topic_0150354069_p583194512587"></a><a name="zh-cn_topic_0150354069_p583194512587"></a>出方向</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.831483148314831%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0150354069_p18831144518586"><a name="zh-cn_topic_0150354069_p18831144518586"></a><a name="zh-cn_topic_0150354069_p18831144518586"></a>TCP</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.781178117811782%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0150354069_p178311145195814"><a name="zh-cn_topic_0150354069_p178311145195814"></a><a name="zh-cn_topic_0150354069_p178311145195814"></a>443</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.512151215121513%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0150354069_p17831345105816"><a name="zh-cn_topic_0150354069_p17831345105816"></a><a name="zh-cn_topic_0150354069_p17831345105816"></a>100.125.0.0/16</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.61376137613761%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0150354069_p483164565813"><a name="zh-cn_topic_0150354069_p483164565813"></a><a name="zh-cn_topic_0150354069_p483164565813"></a>采集监控数据到云监控服务端。</p>
    </td>
    </tr>
    </tbody>
    </table>


