# 手动配置Agent<a name="ZH-CN_TOPIC_0085245601"></a>

## 操作场景<a name="zh-cn_topic_0078544025_section10035481163223"></a>

用户成功安装Agent插件后，需要修改相关配置文件，用于上报监控指标和心跳数据。

## 前提条件<a name="zh-cn_topic_0078544025_section8243987182032"></a>

已成功安装Agent插件。

## 操作步骤<a name="zh-cn_topic_0078544025_section14276669182022"></a>

1.  使用root账号，登录ECS或BMS。
2.  执行以下命令，切换至Agent安装路径的bin下。

    **cd /usr/local/telescope/bin**

3.  修改配置文件conf.json。
    1.  执行以下命令，打开配置文件conf.json。

        **vi conf.json**

    2.  修改文件中的参数，具体参数请参见[表1](#zh-cn_topic_0078544025_table6225399118403)。

        ```
        {
            "InstanceId":"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
            "ProjectId": "b5b92ee0xxxxxxxxxxxxxxxxcab92396",
            "AccessKey": "QZ0XGJXFxxxxxxxxT65R",
            "SecretKey": "lEv2aXAGwxxxxxxxxxxxxxxxxxxxxF8t0Bf18Tn2",
            "RegionId": "cn-north-1",
            "ClientPort": 0,
            "PortNum": 200
        }
        ```

        **表 1**  公共配置参数

        <a name="zh-cn_topic_0078544025_table6225399118403"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0078544025_row1372578218403"><th class="cellrowborder" valign="top" width="16.99%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0078544025_p3804652818403"><a name="zh-cn_topic_0078544025_p3804652818403"></a><a name="zh-cn_topic_0078544025_p3804652818403"></a>参数</p>
        </th>
        <th class="cellrowborder" valign="top" width="83.00999999999999%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0078544025_p6186991018403"><a name="zh-cn_topic_0078544025_p6186991018403"></a><a name="zh-cn_topic_0078544025_p6186991018403"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0078544025_row4540685018403"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0078544025_p5407620118403"><a name="zh-cn_topic_0078544025_p5407620118403"></a><a name="zh-cn_topic_0078544025_p5407620118403"></a>InstanceId</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0078544025_p1809618118403"><a name="zh-cn_topic_0078544025_p1809618118403"></a><a name="zh-cn_topic_0078544025_p1809618118403"></a>ECS或BMS ID，可通过登录管理控制台，在弹性云服务器ECS或裸金属服务器BMS列表中查看。</p>
        <div class="note" id="zh-cn_topic_0078544025_note48453366184034"><a name="zh-cn_topic_0078544025_note48453366184034"></a><a name="zh-cn_topic_0078544025_note48453366184034"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0078544025_ul4659615020823"></a><a name="zh-cn_topic_0078544025_ul4659615020823"></a><ul id="zh-cn_topic_0078544025_ul4659615020823"><li>InstanceId可不用配置，保持"InstanceId":"",即可，若需要配置，请参考下两条。</li><li>该资源ID需保证全局唯一性，即同一个RegionID下Agent使用的InstanceId不能相同，否则系统可能会出现异常。</li><li>InstanceId必须与实际的ECS或BMS资源ID一致，否则云监控界面将看不到对应ECS或BMS资源操作系统监控的数据。</li></ul>
        </div></div>
        </td>
        </tr>
        <tr id="zh-cn_topic_0078544025_row5650459018403"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0078544025_p1346908318403"><a name="zh-cn_topic_0078544025_p1346908318403"></a><a name="zh-cn_topic_0078544025_p1346908318403"></a>ProjectId</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p16105193363717"><a name="p16105193363717"></a><a name="p16105193363717"></a>ProjectId可不用配置，保持"ProjectId": "",即可。若需要配置，请参考已下获取方式。</p>
        <p id="zh-cn_topic_0078544025_p1725395718403"><a name="zh-cn_topic_0078544025_p1725395718403"></a><a name="zh-cn_topic_0078544025_p1725395718403"></a>项目ID，获取方式如下：</p>
        <a name="zh-cn_topic_0078544025_ol2106788818403"></a><a name="zh-cn_topic_0078544025_ol2106788818403"></a><ol id="zh-cn_topic_0078544025_ol2106788818403"><li>登录管理控制台，单击右上角“用户名”，选择“我的凭证”；</li><li>在项目列表中，查看ECS或BMS资源对应的所属区域的项目ID。</li></ol>
        </td>
        </tr>
        <tr id="zh-cn_topic_0078544025_row5766964618403"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0078544025_p4072972518403"><a name="zh-cn_topic_0078544025_p4072972518403"></a><a name="zh-cn_topic_0078544025_p4072972518403"></a>AccessKey/SecretKey</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0078544025_p1077341718403"><a name="zh-cn_topic_0078544025_p1077341718403"></a><a name="zh-cn_topic_0078544025_p1077341718403"></a>访问密钥，获取方式如下：</p>
        <p id="zh-cn_topic_0078544025_p2985188918403"><a name="zh-cn_topic_0078544025_p2985188918403"></a><a name="zh-cn_topic_0078544025_p2985188918403"></a>登录管理控制台，单击右上角“用户名”，选择“我的凭证 &gt; 管理访问秘钥”；</p>
        <a name="ul2261439143714"></a><a name="ul2261439143714"></a><ul id="ul2261439143714"><li>如已有访问密钥，查看创建时下载保存的credentials.csv文件中，获取文件中记录的Key值即可；</li><li>如未创建，则通过“新增访问密钥”可创建新的访问密钥，妥善保存credentials.csv文件，并获取文件中记录的Key值。<div class="notice" id="note1826113397373"><a name="note1826113397373"></a><a name="note1826113397373"></a><span class="noticetitle"> 注意： </span><div class="noticebody"><a name="ul1626113993711"></a><a name="ul1626113993711"></a><ul id="ul1626113993711"><li>为了安全考虑，建议该用户为IAM用户，并且权限仅为CES Administrator和LTS Administrator，请参见<a href="https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0046611269.html" target="_blank" rel="noopener noreferrer">创建用户组并授权</a>、<a href="https://support.huaweicloud.com/qs-iam/iam_01_0031.html" target="_blank" rel="noopener noreferrer">创建IAM用户并加入用户组</a>。</li><li>配置的AccessKey必须在“我的凭证 &gt; 管理访问秘钥”列表中，否则将鉴权失败，云监控界面看不到操作系统监控数据。</li></ul>
        </div></div>
        </li></ul>
        </td>
        </tr>
        <tr id="zh-cn_topic_0078544025_row3457869218403"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0078544025_p4941065418403"><a name="zh-cn_topic_0078544025_p4941065418403"></a><a name="zh-cn_topic_0078544025_p4941065418403"></a>RegionId</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0078544025_p4284005718403"><a name="zh-cn_topic_0078544025_p4284005718403"></a><a name="zh-cn_topic_0078544025_p4284005718403"></a>区域ID，例如：ECS或BMS资源所属区域为“华北-北京一”，则RegionID为“cn-north-1”，其他区域的RegionID详见<a href="https://developer.huaweicloud.com/endpoint.html" target="_blank" rel="noopener noreferrer">https://developer.huaweicloud.com/endpoint.html</a>。</p>
        </td>
        </tr>
        <tr id="row1827144335718"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p152711443145714"><a name="p152711443145714"></a><a name="p152711443145714"></a>ClientPort</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p6746810185819"><a name="p6746810185819"></a><a name="p6746810185819"></a>Agent占用的起始端口号。</p>
        <div class="note" id="note77931415201"><a name="note77931415201"></a><a name="note77931415201"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1879411151207"><a name="p1879411151207"></a><a name="p1879411151207"></a>默认为0，表示随机占用。1-1023为系统保留端口，建议不要配置。</p>
        </div></div>
        </td>
        </tr>
        <tr id="row20886039205718"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p988733945715"><a name="p988733945715"></a><a name="p988733945715"></a>PortNum</p>
        </td>
        <td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p14887173985717"><a name="p14887173985717"></a><a name="p14887173985717"></a>Agent占用的范围的个数。</p>
        <div class="note" id="note132469718113"><a name="note132469718113"></a><a name="note132469718113"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p0247071219"><a name="p0247071219"></a><a name="p0247071219"></a>默认为200，若ClientPort配置5000，则表示在5000-5199端口中随机占用。</p>
        </div></div>
        </td>
        </tr>
        </tbody>
        </table>


4.  修改云监控指标采集模块的配置文件conf\_ces.json。
    1.  执行以下命令，打开公共配置文件conf\_ces.json。

        **vi conf\_ces.json**

    2.  修改文件中的参数，具体参数请参见[表2](#zh-cn_topic_0078544025_table21263594191717)。

        ```
        {
          "Endpoint": "https://ces.cn-north-1.myhuaweicloud.com"
        }
        ```

        **表 2**  指标采集模块参数配置

        <a name="zh-cn_topic_0078544025_table21263594191717"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0078544025_row54283771191717"><th class="cellrowborder" valign="top" width="21.86%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0078544025_p34909346191717"><a name="zh-cn_topic_0078544025_p34909346191717"></a><a name="zh-cn_topic_0078544025_p34909346191717"></a>参数</p>
        </th>
        <th class="cellrowborder" valign="top" width="78.14%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0078544025_p9084806191717"><a name="zh-cn_topic_0078544025_p9084806191717"></a><a name="zh-cn_topic_0078544025_p9084806191717"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0078544025_row64780686191717"><td class="cellrowborder" valign="top" width="21.86%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0078544025_p12744227191717"><a name="zh-cn_topic_0078544025_p12744227191717"></a><a name="zh-cn_topic_0078544025_p12744227191717"></a><strong id="zh-cn_topic_0078544025_b47589181191717"><a name="zh-cn_topic_0078544025_b47589181191717"></a><a name="zh-cn_topic_0078544025_b47589181191717"></a>Endpoint</strong></p>
        </td>
        <td class="cellrowborder" valign="top" width="78.14%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0078544025_p29518480191717"><a name="zh-cn_topic_0078544025_p29518480191717"></a><a name="zh-cn_topic_0078544025_p29518480191717"></a>ECS或BMS资源所属区域的云监控Endpoint URL，例如：ECS或BMS资源所属区域为“华北-北京一”，则URL中使用“ces.cn-north-1.myhuaweicloud.com”，其他区域的Endpoint取值详见<a href="https://developer.huaweicloud.com/endpoint.html" target="_blank" rel="noopener noreferrer">https://developer.huaweicloud.com/endpoint.html</a>。</p>
        </td>
        </tr>
        </tbody>
        </table>

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >Agent插件配置完成后，因监控数据暂未上报，插件状态仍显示“未安装”，等待3-5分钟，刷新即可。  



