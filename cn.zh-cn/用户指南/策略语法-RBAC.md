# 策略语法：RBAC<a name="ZH-CN_TOPIC_0172200272"></a>

## 策略结构<a name="section1661242202715"></a>

策略结构包括：策略版本号（Version）、策略授权语句（Statement）和策略依赖（Depends）。

**图 1**  RBAC的策略结构<a name="fig2641112616326"></a>  
![](figures/RBAC的策略结构.png "RBAC的策略结构")

## 策略语法<a name="section1030510262812"></a>

如下以云监控服务的“CES Administrator”为例，说明RBAC策略语法。

**图 2**  设置策略<a name="fig116861358113111"></a>  
![](figures/设置策略.png "设置策略")

```
{
        "Version": "1.0",
        "Statement": [
                {
                        "Effect": "Allow",
                        "Action": [
                                "CES:Alarm:*",
                                "CES:Metrics:*",
                                "CES:Notification:*",
                                "CES:Generic:*"
                        ]
                }
        ],
        "Depends": [
                {
                        "catalog": "BASE",
                        "display_name": "Tenant Guest"
                }
        ]
}
```

<a name="table4805855114411"></a>
<table><thead align="left"><tr id="row8886195594416"><th class="cellrowborder" colspan="2" valign="top" id="mcps1.1.5.1.1"><p id="p208861355114419"><a name="p208861355114419"></a><a name="p208861355114419"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" id="mcps1.1.5.1.2"><p id="p17886165510447"><a name="p17886165510447"></a><a name="p17886165510447"></a>含义</p>
</th>
<th class="cellrowborder" valign="top" id="mcps1.1.5.1.3"><p id="p1388655514447"><a name="p1388655514447"></a><a name="p1388655514447"></a>值</p>
</th>
</tr>
</thead>
<tbody><tr id="row3886655114415"><td class="cellrowborder" colspan="2" valign="top" headers="mcps1.1.5.1.1 "><p id="p12886155154416"><a name="p12886155154416"></a><a name="p12886155154416"></a>Version</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.2 "><p id="p1988635512447"><a name="p1988635512447"></a><a name="p1988635512447"></a>策略的版本</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.3 "><p id="p8886115564418"><a name="p8886115564418"></a><a name="p8886115564418"></a>固定为“1.0”</p>
</td>
</tr>
<tr id="row5887185515441"><td class="cellrowborder" rowspan="2" valign="top" width="16.24162416241624%" headers="mcps1.1.5.1.1 "><p id="p128871755134412"><a name="p128871755134412"></a><a name="p128871755134412"></a>Statement</p>
</td>
<td class="cellrowborder" valign="top" width="18.491849184918493%" headers="mcps1.1.5.1.1 "><p id="p08878555448"><a name="p08878555448"></a><a name="p08878555448"></a>Action</p>
</td>
<td class="cellrowborder" valign="top" width="27.892789278927893%" headers="mcps1.1.5.1.2 "><p id="p178871955184419"><a name="p178871955184419"></a><a name="p178871955184419"></a>定义对云监控服务的具体操作。</p>
</td>
<td class="cellrowborder" valign="top" width="37.37373737373737%" headers="mcps1.1.5.1.3 "><p id="p2088785524410"><a name="p2088785524410"></a><a name="p2088785524410"></a>格式为：服务名:资源类型:操作</p>
<p id="p58871955144410"><a name="p58871955144410"></a><a name="p58871955144410"></a>"CES:*:*"，表示对云监控服务的所有操作，其中CES为服务名缩写，表示云监控服务；“*”为通配符，表示对所有的资源类型可以执行所有操作。</p>
</td>
</tr>
<tr id="row188785524410"><td class="cellrowborder" valign="top" headers="mcps1.1.5.1.1 "><p id="p1887755154417"><a name="p1887755154417"></a><a name="p1887755154417"></a>Effect</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.1 "><p id="p1788719556444"><a name="p1788719556444"></a><a name="p1788719556444"></a>定义Action中所包含的具体操作是否允许执行。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.2 "><a name="ul188871455134417"></a><a name="ul188871455134417"></a><ul id="ul188871455134417"><li>Allow：允许执行。</li><li>Deny：不允许执行。</li></ul>
</td>
</tr>
<tr id="row1588715544411"><td class="cellrowborder" rowspan="2" valign="top" width="16.24162416241624%" headers="mcps1.1.5.1.1 "><p id="p1688715555445"><a name="p1688715555445"></a><a name="p1688715555445"></a>Depends</p>
</td>
<td class="cellrowborder" valign="top" width="18.491849184918493%" headers="mcps1.1.5.1.1 "><p id="p38871055154411"><a name="p38871055154411"></a><a name="p38871055154411"></a>catalog</p>
</td>
<td class="cellrowborder" valign="top" width="27.892789278927893%" headers="mcps1.1.5.1.2 "><p id="p12887115544418"><a name="p12887115544418"></a><a name="p12887115544418"></a>依赖的策略的所属服务。</p>
</td>
<td class="cellrowborder" valign="top" width="37.37373737373737%" headers="mcps1.1.5.1.3 "><p id="p18887185574414"><a name="p18887185574414"></a><a name="p18887185574414"></a>服务名称</p>
<p id="p2088795524414"><a name="p2088795524414"></a><a name="p2088795524414"></a>例如：BASE</p>
</td>
</tr>
<tr id="row38871155174412"><td class="cellrowborder" valign="top" headers="mcps1.1.5.1.1 "><p id="p3887355204419"><a name="p3887355204419"></a><a name="p3887355204419"></a>display_name</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.1 "><p id="p12887655154413"><a name="p12887655154413"></a><a name="p12887655154413"></a>依赖的策略的名称。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.2 "><p id="p158887551446"><a name="p158887551446"></a><a name="p158887551446"></a>权限名称</p>
<p id="p688825519446"><a name="p688825519446"></a><a name="p688825519446"></a>例如：Tenant Administrator</p>
</td>
</tr>
</tbody>
</table>

