# Agent安装配置方式说明<a name="zh-cn_topic_0078544023"></a>

安装Agent方式有如下几种，你可以根据你所使用的服务的操作系统类型、是否有多个服务器以及个人习惯选择任何一种或多种安装方式：

<a name="table127591910125719"></a>
<table><thead align="left"><tr id="row137601104571"><th class="cellrowborder" valign="top" width="26.16%" id="mcps1.1.5.1.1"><p id="p1272294119012"><a name="p1272294119012"></a><a name="p1272294119012"></a>安装场景</p>
</th>
<th class="cellrowborder" valign="top" width="14.96%" id="mcps1.1.5.1.2"><p id="p068819491808"><a name="p068819491808"></a><a name="p068819491808"></a>支持的服务</p>
</th>
<th class="cellrowborder" valign="top" width="29.73%" id="mcps1.1.5.1.3"><p id="p17601310195713"><a name="p17601310195713"></a><a name="p17601310195713"></a>参考章节</p>
</th>
<th class="cellrowborder" valign="top" width="29.15%" id="mcps1.1.5.1.4"><p id="p1125138338"><a name="p1125138338"></a><a name="p1125138338"></a>约束和限制</p>
</th>
</tr>
</thead>
<tbody><tr id="row11760191019579"><td class="cellrowborder" valign="top" width="26.16%" headers="mcps1.1.5.1.1 "><p id="p1576014107579"><a name="p1576014107579"></a><a name="p1576014107579"></a>安装Agent（Linux）</p>
</td>
<td class="cellrowborder" valign="top" width="14.96%" headers="mcps1.1.5.1.2 "><p id="p9761181017576"><a name="p9761181017576"></a><a name="p9761181017576"></a>ECS、BMS</p>
</td>
<td class="cellrowborder" valign="top" width="29.73%" headers="mcps1.1.5.1.3 "><p id="p47611410125719"><a name="p47611410125719"></a><a name="p47611410125719"></a><a href="在ECS-BMS中安装配置Agent（Linux）.md">在ECS/BMS中安装配置Agent（Linux）</a></p>
</td>
<td class="cellrowborder" valign="top" width="29.15%" headers="mcps1.1.5.1.4 "><p id="p113171303312"><a name="p113171303312"></a><a name="p113171303312"></a>-</p>
</td>
</tr>
<tr id="row1376101016575"><td class="cellrowborder" valign="top" width="26.16%" headers="mcps1.1.5.1.1 "><p id="p83331233125718"><a name="p83331233125718"></a><a name="p83331233125718"></a>安装Agent（Windows）</p>
</td>
<td class="cellrowborder" valign="top" width="14.96%" headers="mcps1.1.5.1.2 "><p id="p1568811495013"><a name="p1568811495013"></a><a name="p1568811495013"></a>ECS</p>
</td>
<td class="cellrowborder" valign="top" width="29.73%" headers="mcps1.1.5.1.3 "><p id="p167613102572"><a name="p167613102572"></a><a name="p167613102572"></a><a href="在ECS中安装配置Agent（Windows）.md">在ECS中安装配置Agent（Windows）</a></p>
</td>
<td class="cellrowborder" valign="top" width="29.15%" headers="mcps1.1.5.1.4 "><p id="p1131205333215"><a name="p1131205333215"></a><a name="p1131205333215"></a>-</p>
</td>
</tr>
<tr id="row976161010579"><td class="cellrowborder" valign="top" width="26.16%" headers="mcps1.1.5.1.1 "><p id="p876151019575"><a name="p876151019575"></a><a name="p876151019575"></a>批量安装Agent（Linux）</p>
</td>
<td class="cellrowborder" valign="top" width="14.96%" headers="mcps1.1.5.1.2 "><p id="p2068812491509"><a name="p2068812491509"></a><a name="p2068812491509"></a>ECS</p>
</td>
<td class="cellrowborder" valign="top" width="29.73%" headers="mcps1.1.5.1.3 "><p id="p147611710135715"><a name="p147611710135715"></a><a name="p147611710135715"></a><a href="在ECS中批量安装Agent（Linux）.md">在ECS中批量安装Agent（Linux）</a></p>
</td>
<td class="cellrowborder" valign="top" width="29.15%" headers="mcps1.1.5.1.4 "><p id="p6133139336"><a name="p6133139336"></a><a name="p6133139336"></a>-</p>
</td>
</tr>
</tbody>
</table>

安装Agent依赖说明：

1.  安装Agent依赖DNS的配置和安全组配置，DNS错误或安全组规则不正确会导致Agent包下载失败。因此在安装Agent前需要首先修改DNS的配置并配置安全组规则。
2.  安装Agent后，可以通过“修复插件配置”完成委托配置和文件配置。
3.  当通过“修改插件配置”或其他原因无法完成Agent配置时，您还可以手工配置Agent。
4.  支持安装Agent的操作系统请参见[Agent支持的系统有哪些](https://support.huaweicloud.com/ces_faq/ces_faq_0024.html)。
5.  对于私有镜像，推荐您使用已安装Agent的ECS或BMS制作私有镜像，并使用该私有镜像购买ECS或BMS，并在创建完资源后通过[修复插件配置](https://support.huaweicloud.com/usermanual-ces/zh-cn_topic_0127536712.html)来完成Agent的配置。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >制作的私有镜像不支持跨Region使用，跨Region使用会导致没有监控数据。  


