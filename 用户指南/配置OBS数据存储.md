# 配置OBS数据存储<a name="zh-cn_topic_0084931808"></a>

## 操作场景<a name="section86441647572"></a>

云监控服务各监控指标的原始数据的保留周期为两天，超过保留周期后原始数据将不再保存。您开通对象存储服务（Object Storage Service，以下简称OBS）后，可将原始数据同步保存至OBS，以保存更长时间。

本章节介绍如何配置数据存储。

## 前提条件<a name="section13948718173426"></a>

-   已开启云服务。
-   已开通对象存储服务。

## 操作步骤<a name="section3571284110915"></a>

1.  登录管理控制台。
2.  单击“管理与部署 \> 云监控服务”。
3.  单击页面左侧导航栏的“云服务监控”，进入“云服务监控”页面，选择待查看的云服务资源所在行的“配置数据存储”，进入“配置数据存储”页面。

    或单击页面左侧的“主机监控”，选择待查看的ECS资源所在行的“更多 \> 配置数据存储”，进入“配置数据存储”页面。

4.  （可选）批量配置数据存储。

    在“云服务监控”页面，勾选需要“配置数据存储”的云服务资源，单击“批量配置数据存储”，进入“批量配置数据存储”页面。

    或在“主机监控”页面，勾选需要“配置数据存储”弹性云服务器，单击“批量配置数据存储”，进入“批量配置数据存储”页面。

5.  在“配置数据存储”或“批量配置数据存储”页面，按照[表1](#table17500185694010)配置参数：

    **表 1**  配置数据存储参数

    <a name="table17500185694010"></a>
    <table><thead align="left"><tr id="row450015610409"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.4.1.1"><p id="p1500756124013"><a name="p1500756124013"></a><a name="p1500756124013"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="44%" id="mcps1.2.4.1.2"><p id="p1500256174013"><a name="p1500256174013"></a><a name="p1500256174013"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="39%" id="mcps1.2.4.1.3"><p id="p118911050164210"><a name="p118911050164210"></a><a name="p118911050164210"></a>样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row145001956164011"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p145008565405"><a name="p145008565405"></a><a name="p145008565405"></a>OBS转储</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p4500195644017"><a name="p4500195644017"></a><a name="p4500195644017"></a>是否配置OBS转储，可选择“转储”和“不转储”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p18919508421"><a name="p18919508421"></a><a name="p18919508421"></a>转储</p>
    </td>
    </tr>
    <tr id="row15500185619400"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p25001056154019"><a name="p25001056154019"></a><a name="p25001056154019"></a>新创建OBS桶</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p950012569403"><a name="p950012569403"></a><a name="p950012569403"></a>若已有OBS桶，可不用创建。</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p15891850144215"><a name="p15891850144215"></a><a name="p15891850144215"></a>是</p>
    </td>
    </tr>
    <tr id="row19500175634017"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p750016568402"><a name="p750016568402"></a><a name="p750016568402"></a>转储OBS桶</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p1586718424717"><a name="p1586718424717"></a><a name="p1586718424717"></a>若没有OBS桶，输入需要创建的OBS桶名。</p>
    <p id="p5500756184012"><a name="p5500756184012"></a><a name="p5500756184012"></a>已有OBS桶时，选择已有的桶。</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1289155019420"><a name="p1289155019420"></a><a name="p1289155019420"></a>ecs-0615</p>
    </td>
    </tr>
    <tr id="row1550055616403"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p35004562402"><a name="p35004562402"></a><a name="p35004562402"></a>监控数据文件前缀</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p25001156164014"><a name="p25001156164014"></a><a name="p25001156164014"></a>通过设置监控数据文件前缀可以方便您区分OBS桶中的云监控服务数据文件与其他普通文件。</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p17892150154216"><a name="p17892150154216"></a><a name="p17892150154216"></a>ecs-0615</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   选中的桶会将读写策略授权给云监控服务，请谨慎修改桶策略，防止转储失败。  
    >-   为了确保安全，选择已有的桶时请选择“存储类型”为标准存储，并且“桶策略”为私有的桶。  
    >-   如果配置的转储策略处于关闭状态七天以上，会默认被清除。若用户需要使用，需重新配置策略。  
    >-   如果用户账户被冻结2小时以上，转储OBS开关会被关闭。若用户需要使用，需要解冻账户并重新打开转储OBS开关。  

6.  单击“确定”，完成配置数据存储。

    配置完数据存储后，系统会在每天的2-4-6-8-10-12-14-16-18-20-22-24整点自动将监控数据转储到OBS桶中。


