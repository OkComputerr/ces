# 在ECS中批量安装Agent（Linux）<a name="ZH-CN_TOPIC_0127544062"></a>

## 操作场景<a name="zh-cn_topic_0111157443_section476316142516"></a>

本章节指导用户在已有的大量弹性云服务器（Linux）上批量安装Agent。

## 操作流程<a name="section149797195411"></a>

选择其中一台ECS绑定弹性IP后，参照[在ECS/BMS中安装配置Agent（Linux）](在ECS-BMS中安装配置Agent（Linux）.md)安装Agent并配置，确保数据采集正常。将此ECS作为跳板机通过批量执行脚本依次将Agent包和配置文件拷贝、解压、执行安装到其他ECS中。

>![](public_sys-resources/icon-notice.gif) **须知：**   
>-   批量安装的ECS需同属一个VPC。  
>-   Windows版本暂不支持批量安装Agent。  
>-   BMS暂不支持批量安装Agent。  

## 前提条件<a name="zh-cn_topic_0111157443_section57291745182517"></a>

-   已收集需要安装Agent的所有ECS的IP地址，按照iplist.txt格式整理好，并上传到第一台机器的/usr/local目录下。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >iplist.txt格式示例如下所示（多台ECS密码一致，可只填写IP）。  
    >```  
    >192.168.1.1  
    >192.168.1.2  
    >```  
    >多台ECS密码不同，建议IP、ID、密码都填写，ID与密码之间用空格隔开。  
    >样例中abcd为密码，请按实际值填写。  
    >```  
    >192.168.1.1:bdf784cb-xxxx-xxxx-xxxx-bf0a99d8d486 abcd  
    >192.168.1.2:cgvfa4e4-xxxx-xxxx-xxxx-b32231553926 abcd  
    >```  


## 操作步骤<a name="zh-cn_topic_0111157443_section335374517325"></a>

1.  使用Putty以root用户登录到已安装Agent的弹性云服务器中。
2.  执行如下命令，下载并安装batchInstallAgent.tar.gz。

    华北-北京一：

    **cd /usr/local && wget https://telescope.obs.cn-north-1.myhuaweicloud.com/scripts/agentBatchPackage.sh && chmod 755 agentBatchPackage.sh && ./agentBatchPackage.sh**

    华北-北京四：

    **cd /usr/local && wget https://telescope-cn-north-4.**obs.**myhuaweicloud.com/scripts/agentBatchPackage.sh && chmod 755 agentBatchPackage.sh && ./agentBatchPackage.sh**

    arm通用计算型：

    **cd /usr/local && wget https://telescope-cn-north-4.obs.myhuaweicloud.com/scripts/agentBatchPackageARM.sh && chmod 755 agentBatchPackageARM.sh && ./agentBatchPackageARM.sh**

    华南-广州：

    **cd /usr/local && wget https://telescope-cn-south-1.obs.cn-south-1.myhuaweicloud.com/scripts/agentBatchPackage.sh && chmod 755 agentBatchPackage.sh && ./agentBatchPackage.sh**

    华东-上海二：

    **cd /usr/local && wget https://telescope-cn-east-2.obs.cn-east-2.myhuaweicloud.com/scripts/agentBatchPackage.sh && chmod 755 agentBatchPackage.sh && ./agentBatchPackage.sh**

    华东-上海一：

    **cd /usr/local && wget --no-check-certificate https://obs.cn-east-3.myhuaweicloud.com/uniagent-cn-east-3/script/uniagent\_patch\_installer\_amd64 && chmod +x uniagent\_patch\_installer && ./uniagent\_patch\_installer\_amd64 -c "cd /usr/local && wget --no-check-certificate https://obs.cn-east-3.myhuaweicloud.com/uniagent-cn-east-3/script/uniagent\_install\_amd64.sh && bash uniagent\_install\_amd64.sh"**

    亚太-香港：

    **cd /usr/local && wget https://telescope-ap-southeast-1.obs.ap-southeast-1.myhuaweicloud.com/scripts/agentBatchPackage.sh && chmod 755 agentBatchPackage.sh && ./agentBatchPackage.sh**

    亚太-曼谷：

    **cd /usr/local && wget https://telescope-ap-southeast-2.obs.ap-southeast-2.myhuaweicloud.com/scripts/agentBatchPackage.sh && chmod 755 agentBatchPackage.sh && ./agentBatchPackage.sh**

    亚太-新加坡：

    **cd /usr/local && wget https://telescope-ap-southeast-3.obs.ap-southeast-3.myhuaweicloud.com/scripts/agentBatchPackage.sh && chmod 755 agentBatchPackage.sh && ./agentBatchPackage.sh**

    非洲-约翰内斯堡：

    **cd /usr/local && wget https://telescope-af-south-1.obs.af-south-1.myhuaweicloud.com/scripts/agentBatchPackage.sh && chmod 755 agentBatchPackage.sh && ./agentBatchPackage.sh**

3.  执行如下命令，运行脚本并输入密码（多台ECS密码一致）。

    **cd /usr/local && ./batchInstall.sh $password**

    >![](public_sys-resources/icon-notice.gif) **须知：**   
    >-   如果配置的iplist.txt中涉及多个密码则多次输入上述命令和密码，密码不对的ECS则会安装失败。  
    >-   多台ECS密码不同时，请执行**cd /usr/local && ./batchInstall.sh。**  
    >-   脚本执行过程中需保证ECS正常开机状态。  

4.  安装完成后，登录云监控服务管理控制台，单击左侧导航栏的“主机监控”。

    查看所有已安装Agent的弹性云服务器列表。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >Agent插件配置完成后，因监控数据暂未上报，插件状态仍显示“未安装”，等待3-5分钟，刷新即可。  

5.  在“主机监控”页面全选ECS后，单击“修复插件配置”。
6.  在弹出的页面中单击“一键修复”。
7.  （可选）安装完成后如果不需要pexpect模块，则执行如下命令，到python安装目录下删除pexepct 和ptyprocess模块。

    **cd /usr/lib/python2.7/site-packages**

    **rm pexpect-3.2-py2.7.egg-info -f**

    **rm ptyprocess-0.5.2-py2.7.egg-info -f**

    **rm pexpect -rf**

    **rm ptyprocess -rf**


