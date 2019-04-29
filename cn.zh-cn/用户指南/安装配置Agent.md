# 安装配置Agent<a name="ZH-CN_TOPIC_0110258146"></a>

## 前提条件<a name="section843453701616"></a>

-   已配置DNS与安全组，配置DNS与安全组请参见[修改DNS与添加安全组](修改DNS与添加安全组-1.md)。
-   确保[操作步骤](#section1251913413419)中的安装目录都有读写权限，并且安装成功后的Telescope进程不会被其他软件关闭。
-   已获取Agent安装包（windows）。

    **表 1**  安装包路径

    <a name="zh-cn_topic_0078544024_table3148844917055"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0078544024_row5377394617055"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0078544024_p6072235217055"><a name="zh-cn_topic_0078544024_p6072235217055"></a><a name="zh-cn_topic_0078544024_p6072235217055"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="8%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0078544024_p1956351617055"><a name="zh-cn_topic_0078544024_p1956351617055"></a><a name="zh-cn_topic_0078544024_p1956351617055"></a>格式</p>
    </th>
    <th class="cellrowborder" valign="top" width="72%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0078544024_p4114093117055"><a name="zh-cn_topic_0078544024_p4114093117055"></a><a name="zh-cn_topic_0078544024_p4114093117055"></a>下载路径</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0078544024_row4408113517055"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0078544024_p1380221617055"><a name="zh-cn_topic_0078544024_p1380221617055"></a><a name="zh-cn_topic_0078544024_p1380221617055"></a>Windows 64位Agent安装包</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0078544024_p4423771717055"><a name="zh-cn_topic_0078544024_p4423771717055"></a><a name="zh-cn_topic_0078544024_p4423771717055"></a>zip</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.4.1.3 "><p id="p13161429133514"><a name="p13161429133514"></a><a name="p13161429133514"></a>华北-北京一：<a href="https://telescope.obs.cn-north-1.myhuaweicloud.com/agent/telescope_windows_amd64.zip" target="_blank" rel="noopener noreferrer">https://telescope.obs.cn-north-1.myhuaweicloud.com/agent/telescope_windows_amd64.zip</a></p>
    <p id="p12421810158"><a name="p12421810158"></a><a name="p12421810158"></a>华北-北京四：<a href="https://telescope-cn-north-4.obs.cn-north-4.myhuaweicloud.com/agent/telescope_windows_amd64.zip" target="_blank" rel="noopener noreferrer">https://telescope-cn-north-4.obs.cn-north-4.myhuaweicloud.com/agent/telescope_windows_amd64.zip</a></p>
    <p id="p14317929163510"><a name="p14317929163510"></a><a name="p14317929163510"></a>华南-广州：<a href="https://telescope-cn-south-1.obs.cn-south-1.myhuaweicloud.com/agent/telescope_windows_amd64.zip" target="_blank" rel="noopener noreferrer">https://telescope-cn-south-1.obs.cn-south-1.myhuaweicloud.com/agent/telescope_windows_amd64.zip</a></p>
    <p id="p531762920357"><a name="p531762920357"></a><a name="p531762920357"></a>华东-上海二：<a href="https://telescope-cn-east-2.obs.cn-east-2.myhuaweicloud.com/agent/telescope_windows_amd64.zip" target="_blank" rel="noopener noreferrer">https://telescope-cn-east-2.obs.cn-east-2.myhuaweicloud.com/agent/telescope_windows_amd64.zip</a></p>
    <p id="p575185010570"><a name="p575185010570"></a><a name="p575185010570"></a>亚太-香港：<a href="https://telescope-ap-southeast-1.obs.ap-southeast-1.myhuaweicloud.com/agent/telescope_windows_amd64.zip">https://telescope-ap-southeast-1.obs.ap-southeast-1.myhuaweicloud.com/agent/telescope_windows_amd64.zip</a></p>
    <p id="p07931526201115"><a name="p07931526201115"></a><a name="p07931526201115"></a>亚太-曼谷：<a href="https://telescope-ap-southeast-2.obs.ap-southeast-2.myhuaweicloud.com/agent/telescope_windows_amd64.zip">https://telescope-ap-southeast-2.obs.ap-southeast-2.myhuaweicloud.com/agent/telescope_windows_amd64.zip</a></p>
    </td>
    </tr>
    </tbody>
    </table>


## 操作步骤<a name="section1251913413419"></a>

1.  VNC方式登录Windows弹性云服务器。
2.  在浏览器地址栏输入Agent安装包地址，下载并保存安装包。
3.  创建安装包存放目录（如D:\\Agent），解压Agent安装包telescope\_windows\_amd64.zip到该目录下。
4.  双击执行install.bat脚本，安装并启动Agent。

    当界面显示Install service success时，说明Agent安装成功并启动。

    **图 1**  安装Agent<a name="fig15988419512"></a>  
    ![](figures/安装Agent.png "安装Agent")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >Agent插件配置完成后，因监控数据暂未上报，插件状态仍显示“未安装”，等待3-5分钟，刷新即可。  

5.  安装完成后，您可以选择进入主机监控界面，勾选需要配置插件的主机，单击"修复插件配置"，在弹出页面上，单击"一键修复"，完成配置Agent。

    **图 2**  修复插件配置<a name="fig62115119195"></a>  
    ![](figures/修复插件配置-1.png "修复插件配置-1")

    如需手动配置Agent。打开telescope\_windows\_amd64\\bin文件夹下的conf.json文件，配置Agent具体参数，参数说明请参见[表1](手动配置Agent.md#zh-cn_topic_0078544025_table6225399118403)。然后双击执行install.bat脚本。

    ```
    {
        "InstanceId":"",
        "ProjectId": "",
        "AccessKey": "",
        "SecretKey": "",
        "RegionId": "cn-north-1",
        "ClientPort": 0,
        "PortNum": 200
    }
    ```


