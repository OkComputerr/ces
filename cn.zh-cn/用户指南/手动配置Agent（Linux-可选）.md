# 手动配置Agent（Linux，可选）<a name="zh-cn_topic_0085245601"></a>

## 操作场景<a name="zh-cn_topic_0078544025_section10035481163223"></a>

用户成功安装Agent插件后，推荐您采用“修复插件配置”方式配置Agent。如果“修复插件”配置不成功或其他原因，你可以采用本章节提供的手工方式配置Agent。

本章节以ECS为例介绍如何修改DNS和添加安全组，BMS操作步骤类似。

## 前提条件<a name="zh-cn_topic_0078544025_section8243987182032"></a>

已成功安装Agent插件。

## 操作步骤<a name="zh-cn_topic_0078544025_section14276669182022"></a>

1.  使用root账号，登录ECS。
2.  执行以下命令，切换至Agent安装路径的bin下。

    **cd /usr/local/telescope/bin**

3.  修改配置文件conf.json。
    1.  执行以下命令，打开配置文件conf.json。

        **vi conf.json**

    2.  修改文件中的参数，具体参数请参见[表1](#table98030118576)。

        **ECS配置参数**

        ```
        {
            "InstanceId":"XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
            "ProjectId": "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
            "AccessKey": "XXXXXXXXXXXXXXXXXXXX",
            "SecretKey": "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
            "RegionId": "cn-north-1",
            "ClientPort": 0,
            "PortNum": 200
        }
        ```

        **BMS配置参数**

        ```
        {
            "InstanceId":"XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
            "ProjectId": "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
            "AccessKey": "XXXXXXXXXXXXXXXXXXXX",
            "SecretKey": "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
            "RegionId": "cn-north-1",
            "ClientPort": 0,
            "PortNum": 200,
            "BmsFlag": true
        }
        ```

        **表 1**  公共配置参数

        <a name="table98030118576"></a>
        <table><thead align="left"><tr id="row480019135712"><th class="cellrowborder" valign="top" width="16.99%" id="mcps1.2.3.1.1"><p id="p18800161195711"><a name="p18800161195711"></a><a name="p18800161195711"></a>参数</p>
        </th>
        <th class="cellrowborder" valign="top" width="83.00999999999999%" id="mcps1.2.3.1.2"><p id="p08007155712"><a name="p08007155712"></a><a name="p08007155712"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="row198006116573"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p0800416571"><a name="p0800416571"></a><a name="p0800416571"></a>InstanceId</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p68009185715"><a name="p68009185715"></a><a name="p68009185715"></a>ECS ID，可通过登录管理控制台，在弹性云服务器ECS列表中查看。</p>
        <div class="note" id="note680015118574"><a name="note680015118574"></a><a name="note680015118574"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="ul8800181135717"></a><a name="ul8800181135717"></a><ul id="ul8800181135717"><li>InstanceId可不用配置，保持"InstanceId":"",即可，若需要配置，请参考下两条。</li><li>该资源ID需保证全局唯一性，即同一个RegionID下Agent使用的InstanceId不能相同，否则系统可能会出现异常。</li><li>InstanceId必须与实际的ECS或BMS资源ID一致，否则云监控服务界面将看不到对应ECS或BMS资源操作系统监控的数据。</li></ul>
        </div></div>
        </td>
        </tr>
        <tr id="row98019195711"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p1180015175716"><a name="p1180015175716"></a><a name="p1180015175716"></a>ProjectId</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p128016165719"><a name="p128016165719"></a><a name="p128016165719"></a>ProjectId可不用配置，保持"ProjectId": "",即可。若需要配置，请参考已下获取方式。</p>
        <p id="p178014119572"><a name="p178014119572"></a><a name="p178014119572"></a>项目ID，获取方式如下：</p>
        <a name="ol6801912572"></a><a name="ol6801912572"></a><ol id="ol6801912572"><li>登录管理控制台，单击右上角“用户名”，选择“我的凭证”；</li><li>在项目列表中，查看ECS或BMS资源对应的所属区域的项目ID。</li></ol>
        </td>
        </tr>
        <tr id="row28022175713"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p6801101195712"><a name="p6801101195712"></a><a name="p6801101195712"></a>AccessKey/SecretKey</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p128012116575"><a name="p128012116575"></a><a name="p128012116575"></a>访问密钥，获取方式如下：</p>
        <p id="p138019118571"><a name="p138019118571"></a><a name="p138019118571"></a>登录管理控制台，单击右上角“用户名”，选择“我的凭证 &gt; 访问密钥”；</p>
        <a name="ul080117135719"></a><a name="ul080117135719"></a><ul id="ul080117135719"><li>如已有访问密钥，查看创建时下载保存的credentials.csv文件中，获取文件中记录的Key值即可；</li><li>如未创建，则通过“新增访问密钥”可创建新的访问密钥，妥善保存credentials.csv文件，并获取文件中记录的Key值。<div class="notice" id="note128011514579"><a name="note128011514579"></a><a name="note128011514579"></a><span class="noticetitle"> 须知： </span><div class="noticebody"><a name="ul6801181175710"></a><a name="ul6801181175710"></a><ul id="ul6801181175710"><li>为了安全考虑，建议该用户为IAM用户，并且权限仅为CES Administrator和LTS Administrator，请参见<a href="https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0046611269.html" target="_blank" rel="noopener noreferrer">创建用户组并授权</a>、<a href="https://support.huaweicloud.com/qs-iam/iam_01_0031.html" target="_blank" rel="noopener noreferrer">创建IAM用户并加入用户组</a>。</li><li>配置的AccessKey必须在“我的凭证 &gt; 访问密钥”列表中，否则将鉴权失败，云监控服务界面看不到操作系统监控数据。</li></ul>
        </div></div>
        </li></ul>
        </td>
        </tr>
        <tr id="row28029111579"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p13802121125711"><a name="p13802121125711"></a><a name="p13802121125711"></a>RegionId</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p0802191165719"><a name="p0802191165719"></a><a name="p0802191165719"></a>区域ID，例如：ECS或BMS资源所属区域为“华北-北京一”，则RegionID为“cn-north-1”，其他区域的RegionID详见<a href="https://developer.huaweicloud.com/endpoint" target="_blank" rel="noopener noreferrer">https://developer.huaweicloud.com/endpoint</a>。</p>
        </td>
        </tr>
        <tr id="row1680331125719"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p168020118574"><a name="p168020118574"></a><a name="p168020118574"></a>ClientPort</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p14802415577"><a name="p14802415577"></a><a name="p14802415577"></a>Agent占用的起始端口号。</p>
        <div class="note" id="note1380316195718"><a name="note1380316195718"></a><a name="note1380316195718"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p15803181125718"><a name="p15803181125718"></a><a name="p15803181125718"></a>默认为0，表示随机占用。1-1023为系统保留端口，建议不要配置。</p>
        </div></div>
        </td>
        </tr>
        <tr id="row148035125713"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p1480391135715"><a name="p1480391135715"></a><a name="p1480391135715"></a>PortNum</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p88031913576"><a name="p88031913576"></a><a name="p88031913576"></a>Agent占用的范围的个数。</p>
        <div class="note" id="note128030119574"><a name="note128030119574"></a><a name="note128030119574"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p180312115571"><a name="p180312115571"></a><a name="p180312115571"></a>默认为200，若ClientPort配置5000，则表示在5000-5199端口中随机占用。</p>
        </div></div>
        </td>
        </tr>
        <tr id="row880320118572"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p88039111577"><a name="p88039111577"></a><a name="p88039111577"></a>BmsFlag</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p158031519573"><a name="p158031519573"></a><a name="p158031519573"></a>BMS需配置此参数为true，ECS配置项中无需配置。</p>
        <p id="p12630104511330"><a name="p12630104511330"></a><a name="p12630104511330"></a>Windows操作系统中无需要配置。</p>
        </td>
        </tr>
        </tbody>
        </table>

4.  修改云监控服务指标采集模块的配置文件conf\_ces.json。
    1.  执行以下命令，打开公共配置文件conf\_ces.json。

        **vi conf\_ces.json**

    2.  修改文件中的参数，修改完成后保存conf\_ces.json文件。具体参数请参见[表2](#zh-cn_topic_0078544025_table21263594191717)。

        ```
        {
          "Endpoint": "https://ces.cn-north-1.myhuaweicloud.com"
        }
        ```

        **表 2**  指标采集模块参数配置

        <a name="zh-cn_topic_0078544025_table21263594191717"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0078544025_row54283771191717"><th class="cellrowborder" valign="top" width="21.98%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0078544025_p34909346191717"><a name="zh-cn_topic_0078544025_p34909346191717"></a><a name="zh-cn_topic_0078544025_p34909346191717"></a>参数</p>
        </th>
        <th class="cellrowborder" valign="top" width="78.02%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0078544025_p9084806191717"><a name="zh-cn_topic_0078544025_p9084806191717"></a><a name="zh-cn_topic_0078544025_p9084806191717"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0078544025_row64780686191717"><td class="cellrowborder" valign="top" width="21.98%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0078544025_p12744227191717"><a name="zh-cn_topic_0078544025_p12744227191717"></a><a name="zh-cn_topic_0078544025_p12744227191717"></a><strong id="zh-cn_topic_0078544025_b47589181191717"><a name="zh-cn_topic_0078544025_b47589181191717"></a><a name="zh-cn_topic_0078544025_b47589181191717"></a>Endpoint</strong></p>
        </td>
        <td class="cellrowborder" valign="top" width="78.02%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0078544025_p29518480191717"><a name="zh-cn_topic_0078544025_p29518480191717"></a><a name="zh-cn_topic_0078544025_p29518480191717"></a>ECS或BMS资源所属区域的云监控服务Endpoint URL，例如：ECS或BMS资源所属区域为“华北-北京一”，则URL中使用“ces.cn-north-1.myhuaweicloud.com”，其他区域的Endpoint取值详见<a href="https://developer.huaweicloud.com/endpoint" target="_blank" rel="noopener noreferrer">https://developer.huaweicloud.com/endpoint</a>。</p>
        </td>
        </tr>
        </tbody>
        </table>

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >-   Agent插件配置完成后，因监控数据暂未上报，插件状态仍显示“未安装”，等待3-5分钟，刷新即可。  
        >-   当插件状态为“运行中”并且监控状态开启时，说明Agent已安装成功并开始采集细粒度监控指标。  



