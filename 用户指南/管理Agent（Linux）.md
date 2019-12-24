# 管理Agent（Linux）<a name="zh-cn_topic_0085245602"></a>

## 查看Agent状态<a name="zh-cn_topic_0078544026_section10100354193654"></a>

登录ECS或BMS，执行以下命令，查看Agent状态。

**service telescoped status**

当系统返回以下内容，则表示Agent为正常运行状态。

```
"Telescope process is running well." 
```

>![](public_sys-resources/icon-note.gif) **说明：**   
>查看、启动、停止和卸载Agent需使用root用户。  

## 启动Agent<a name="zh-cn_topic_0078544026_section9205013194254"></a>

执行以下命令，启动Agent。

**/usr/local/telescope/telescoped start**

## 重启Agent<a name="zh-cn_topic_0078544026_section1592065167"></a>

执行以下命令，重启Agent。

**/usr/local/telescope/telescoped restart**

## 停止Agent<a name="zh-cn_topic_0078544026_section6164118819395"></a>

登录ECS或BMS，执行以下命令，停止Agent。

**service telescoped stop**

>![](public_sys-resources/icon-note.gif) **说明：**   
>如果Telescope安装失败，可能会导致无法正常停止Agent，可通过执行以下命令进一步尝试；  
>**/usr/local/telescope/telescoped stop**  

## 卸载Agent<a name="zh-cn_topic_0078544026_section15609921194423"></a>

用户可手动卸载Agent插件，卸载后云监控服务将不再主动采集ESC或BMS秒级粒度的监控数据。如需再次使用，请参考[在ECS/BMS中安装配置Agent（Linux）](在ECS-BMS中安装配置Agent（Linux）.md)重新安装。

执行以下命令，即可卸载Agent。

**/usr/local/telescope/uninstall.sh**

>![](public_sys-resources/icon-notice.gif) **须知：**   
>重新安装Agent前，请手动清理之前的Agent安装包。  

