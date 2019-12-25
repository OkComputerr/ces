# 安装GPU指标与RAID指标采集插件（Linux）<a name="zh-cn_topic_0101158226"></a>

## 操作场景<a name="section16321812105715"></a>

本章节指导用户安装指标采集插件，用于采集ECS GPU类指标和BMS RAID类指标。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   ECS支持GPU类指标，BMS暂不支持。  
>-   BMS支持RAID类指标，ECS暂不支持。  
>-   若Agent升级到1.0.5及以上版本，对应插件需使用最新的版本，否则会出现指标采集异常。  

## 前提条件<a name="section1091435320510"></a>

-   已安装Agent并处于正常运行状态。
-   GPU类指标采集需弹性云服务器支持GPU。

## 操作步骤<a name="section4190191715589"></a>

1.  使用root账号，登录ECS。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   若要监控BMS的软RAID指标，请登录BMS。  
    >-   以下以安装GPU插件为例，安装监控软RAID插件类似。  

2.  执行以下命令,进入Agent安装路径/usr/local/telescope。

    **cd** **/usr/local/telescope**

3.  执行以下命令,创建plugins文件夹。

    **mkdir** **plugins**

4.  执行以下命令,进入plugins文件夹。

    **cd** **plugins**

5.  执行如下命令，下载采集插件脚本（以下以GPU插件为例）。

    **wget** ****_https://telescope.obs.cn-north-1.myhuaweicloud.com/gpu\_collector_****

    **表 1**  获取插件采集安装包

    <a name="zh-cn_topic_0078544024_table3148844917055"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0078544024_row5377394617055"><th class="cellrowborder" valign="top" width="26%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0078544024_p6072235217055"><a name="zh-cn_topic_0078544024_p6072235217055"></a><a name="zh-cn_topic_0078544024_p6072235217055"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="74%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0078544024_p4114093117055"><a name="zh-cn_topic_0078544024_p4114093117055"></a><a name="zh-cn_topic_0078544024_p4114093117055"></a>下载路径</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0078544024_row4408113517055"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p428593214552"><a name="p428593214552"></a><a name="p428593214552"></a>Linux 64位GPU指标采集插件安装包</p>
    </td>
    <td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p17289419125518"><a name="p17289419125518"></a><a name="p17289419125518"></a>华北-北京一<span>：</span><a href="https://telescope.obs.cn-north-1.myhuaweicloud.com/gpu_collector" target="_blank" rel="noopener noreferrer">https://telescope.obs.cn-north-1.myhuaweicloud.com/gpu_collector</a></p>
    <p id="p3652616121316"><a name="p3652616121316"></a><a name="p3652616121316"></a>华北-北京四<span>：</span><a href="https://telescope-cn-north-4.obs.cn-north-4.myhuaweicloud.com/gpu_collector" target="_blank" rel="noopener noreferrer">https://telescope-cn-north-4.obs.cn-north-4.myhuaweicloud.com/gpu_collector</a></p>
    <p id="p10945142315549"><a name="p10945142315549"></a><a name="p10945142315549"></a>华南-广州：<a href="https://telescope-cn-south-1.obs.cn-south-1.myhuaweicloud.com/gpu_collector" target="_blank" rel="noopener noreferrer">https://telescope-cn-south-1.obs.cn-south-1.myhuaweicloud.com/gpu_collector</a></p>
    <p id="p9945423195411"><a name="p9945423195411"></a><a name="p9945423195411"></a>华东-上海二：<a href="https://telescope-cn-east-2.obs.cn-east-2.myhuaweicloud.com/gpu_collector" target="_blank" rel="noopener noreferrer">https://telescope-cn-east-2.obs.cn-east-2.myhuaweicloud.com/gpu_collector</a></p>
    <p id="p65151012202019"><a name="p65151012202019"></a><a name="p65151012202019"></a>亚太-香港：<a href="https://telescope-ap-southeast-1.obs.ap-southeast-1.myhuaweicloud.com/gpu_collector" target="_blank" rel="noopener noreferrer">https://telescope-ap-southeast-1.obs.ap-southeast-1.myhuaweicloud.com/gpu_collector</a></p>
    <p id="p1027511153160"><a name="p1027511153160"></a><a name="p1027511153160"></a>亚太-曼谷：<a href="https://telescope-ap-southeast-2.obs.ap-southeast-2.myhuaweicloud.com/gpu_collector" target="_blank" rel="noopener noreferrer">https://telescope-ap-southeast-2.obs.ap-southeast-2.myhuaweicloud.com/gpu_collector</a></p>
    <p id="p1956955911716"><a name="p1956955911716"></a><a name="p1956955911716"></a>亚太-新加坡：<a href="https://telescope-ap-southeast-3.obs.ap-southeast-3.myhuaweicloud.com/gpu_collector" target="_blank" rel="noopener noreferrer">https://telescope-ap-southeast-3.obs.ap-southeast-3.myhuaweicloud.com/gpu_collector</a></p>
    </td>
    </tr>
    <tr id="row119822016478"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p59827084713"><a name="p59827084713"></a><a name="p59827084713"></a>Linux 64位RAID指标采集插件安装包</p>
    </td>
    <td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p193828811471"><a name="p193828811471"></a><a name="p193828811471"></a>华北-北京一<span>：</span><a href="https://telescope.obs.cn-north-1.myhuaweicloud.com/raid_monitor.sh" target="_blank" rel="noopener noreferrer">https://telescope.obs.cn-north-1.myhuaweicloud.com/raid_monitor.sh</a></p>
    <p id="p12454812101716"><a name="p12454812101716"></a><a name="p12454812101716"></a>华北-北京四<span>：</span><a href="https://telescope-cn-north-4.obs.cn-north-4.myhuaweicloud.com/raid_monitor.sh" target="_blank" rel="noopener noreferrer">https://telescope-cn-north-4.obs.cn-north-4.myhuaweicloud.com/raid_monitor.sh</a></p>
    <p id="p12138134710541"><a name="p12138134710541"></a><a name="p12138134710541"></a>华南-广州：<a href="https://telescope-cn-south-1.obs.cn-south-1.myhuaweicloud.com/raid_monitor.sh" target="_blank" rel="noopener noreferrer">https://telescope-cn-south-1.obs.cn-south-1.myhuaweicloud.com/raid_monitor.sh</a></p>
    <p id="p1413844718542"><a name="p1413844718542"></a><a name="p1413844718542"></a>华东-上海二：<a href="https://telescope-cn-east-2.obs.cn-east-2.myhuaweicloud.com/raid_monitor.sh" target="_blank" rel="noopener noreferrer">https://telescope-cn-east-2.obs.cn-east-2.myhuaweicloud.com/raid_monitor.sh</a></p>
    <p id="p192042319205"><a name="p192042319205"></a><a name="p192042319205"></a>亚太-香港：<a href="https://telescope-ap-southeast-1.obs.ap-southeast-1.myhuaweicloud.com/raid_monitor.sh" target="_blank" rel="noopener noreferrer">https://telescope-ap-southeast-1.obs.ap-southeast-1.myhuaweicloud.com/raid_monitor.sh</a></p>
    <p id="p984264810165"><a name="p984264810165"></a><a name="p984264810165"></a>亚太-曼谷：<a href="https://telescope-ap-southeast-2.obs.ap-southeast-2.myhuaweicloud.com/raid_monitor.sh" target="_blank" rel="noopener noreferrer">https://telescope-ap-southeast-2.obs.ap-southeast-2.myhuaweicloud.com/raid_monitor.sh</a></p>
    </td>
    </tr>
    </tbody>
    </table>

    [https://telescope-ru-moscow-1.obs.hc.sbercloud.ru/gpu\_collector](https://telescope-ru-moscow-1.obs.hc.sbercloud.ru/gpu_collector)

6.  执行如下命令，添加脚本执行权限。

    **chmod** **755** **gpu\_collector**

7.  执行如下命令，新建conf.json文件并添加配置内容，配置插件路径和指标采集周期crontime（单位：秒）。

    **vi** **conf.json**

    GPU指标插件配置

    ```
    { 
       "plugins": [ 
         { 
           "path": "/usr/local/telescope/plugins/gpu_collector", 
           "crontime": 60 
         }
      ] 
    }
    ```

    RAID指标插件配置

    ```
    { 
       "plugins": [ 
         { 
           "path": "/usr/local/telescope/plugins/raid_monitor.sh", 
           "crontime": 60 
         }
      ] 
    }
    ```

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   path路径后的参数为gpu\_collector和raid\_monitor.sh分别为GPU插件和RAID插件配置内容。  
    >-   插件采集周期为60s，若采集周期配置错误，会导致指标采集异常。  
    >-   插件路径path请勿私自修改，否则指标采集异常。  

8.  打开/usr/local/telescope/bin路径下的conf\_ces.json文件，新增配置项"EnablePlugin"：true，开启插件采集开关。

    ```
    {    
        "Endpoint": "https://ces.cn-north-1.myhuaweicloud.com",
        "EnablePlugin": true
    }
    ```

9.  执行如下命令，重启Agent。

    **/usr/local/telescope/telescoped** **restart**


