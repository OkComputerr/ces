# 修复插件配置（Linux）<a name="ZH-CN_TOPIC_0127536712"></a>

## 操作场景<a name="zh-cn_topic_0085245599_zh-cn_topic_0078544024_section10035481163223"></a>

本章节主要介绍安装Agent后，修复插件配置，免去手动配置Agent的步骤。推荐采用此方法配置Agent。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   "修复插件配置"针对1.0.5及以上版本的Agent，低于该版本请升级Agent后再执行"修复插件配置"，或参考[手动配置Agent（Linux，可选）](手动配置Agent（Linux-可选）.md)手动配置Agent。  
>-   查看Agent版本请参考[如何查询当前正在使用的Agent版本？](https://support.huaweicloud.com/ces_faq/ces_faq_0044.html)。  
>-   "修复插件配置"暂不支持裸金属服务器，裸金属服务器配置Agent，请参见[手动配置Agent（Linux，可选）](手动配置Agent（Linux-可选）.md)章节。  
>-   “华东-上海一”区域已上线一键式授予该区域插件权限功能。您可以单击“主机监控 - 弹性云服务器”页面上方的“一键配置”开启该区域插件权限。开启后，不需要在执行下面步骤。  

## 修改插件配置（ECS）<a name="section106061810131419"></a>

1.  登录管理控制台。
2.  单击“管理与部署 \> 云监控服务 \> 主机监控”。
3.  在主机监控界面，勾选已安装插件的主机。
4.  单击“修复插件配置”。
5.  在弹出页面上，单击“一键修复”。

    当“插件状态”变为“运行中”并且“监控状态”开启时，说明Agent已安装成功并开始采集细粒度监控指标。

    **图 1**  修复ECS插件配置<a name="fig192427475"></a>  
    ![](figures/修复ECS插件配置.png "修复ECS插件配置")


## 修复插件配置（BMS）<a name="section528243961413"></a>

1.  登录管理控制台。
2.  单击“计算 \> 裸金属服务”。
3.  单击已安装插件的主机。
4.  单击“监控”页签。
5.  配置“委托”参数为“CESAgentAutoConfigAgency”。

    如果下拉选项中无CESAgentAutoConfigAgency时，请参考[如何创建委托？](https://support.huaweicloud.com/ces_faq/ces_faq_0028.html)。

6.  单击“提交”。

