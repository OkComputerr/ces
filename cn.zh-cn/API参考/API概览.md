# API概览<a name="ZH-CN_TOPIC_0171212514"></a>

通过使用云监控所提供的接口，您可以完整的使用云监控的所有功能。例如查询指标列表、创建告警规则等。

**表 1**  接口说明

<a name="table5876102613294"></a>
<table><thead align="left"><tr id="row3878122616298"><th class="cellrowborder" valign="top" width="15.72%" id="mcps1.2.5.1.1"><p id="p487811268290"><a name="p487811268290"></a><a name="p487811268290"></a><strong id="b1251874443714"><a name="b1251874443714"></a><a name="b1251874443714"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="14.63%" id="mcps1.2.5.1.2"><p id="p185241222184015"><a name="p185241222184015"></a><a name="p185241222184015"></a><strong id="b4853122913401"><a name="b4853122913401"></a><a name="b4853122913401"></a>子类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="p68781126182914"><a name="p68781126182914"></a><a name="p68781126182914"></a><strong id="b1466274418400"><a name="b1466274418400"></a><a name="b1466274418400"></a>API</strong></p>
</th>
<th class="cellrowborder" valign="top" width="48.22%" id="mcps1.2.5.1.4"><p id="p158781726112914"><a name="p158781726112914"></a><a name="p158781726112914"></a><strong id="b15203449370"><a name="b15203449370"></a><a name="b15203449370"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row10642450201717"><td class="cellrowborder" rowspan="14" valign="top" width="15.72%" headers="mcps1.2.5.1.1 "><p id="p2643250181719"><a name="p2643250181719"></a><a name="p2643250181719"></a>Cloud Eye接口</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="14.63%" headers="mcps1.2.5.1.2 "><p id="p25251422194017"><a name="p25251422194017"></a><a name="p25251422194017"></a>API版本号管理</p>
</td>
<td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p6643175019174"><a name="p6643175019174"></a><a name="p6643175019174"></a><a href="查询API所有版本.md">查询API所有版本</a></p>
</td>
<td class="cellrowborder" valign="top" width="48.22%" headers="mcps1.2.5.1.4 "><p id="p064319508177"><a name="p064319508177"></a><a name="p064319508177"></a>查询云监控支持的API所有版本号。</p>
</td>
</tr>
<tr id="row137731446101711"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p1177414465171"><a name="p1177414465171"></a><a name="p1177414465171"></a><a href="查询API指定版本号.md">查询API指定版本号</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p87741046131719"><a name="p87741046131719"></a><a name="p87741046131719"></a>查询云监控API指定版本号。</p>
</td>
</tr>
<tr id="row148781026122919"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p18525132215407"><a name="p18525132215407"></a><a name="p18525132215407"></a>指标管理</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p128788265295"><a name="p128788265295"></a><a name="p128788265295"></a><a href="查询指标列表.md">查询指标列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="p56591328178"><a name="p56591328178"></a><a name="p56591328178"></a>查询系统当前可监控指标的列表。</p>
</td>
</tr>
<tr id="row98135388177"><td class="cellrowborder" rowspan="5" valign="top" headers="mcps1.2.5.1.1 "><p id="p1552562218408"><a name="p1552562218408"></a><a name="p1552562218408"></a>告警规则管理</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p381383871715"><a name="p381383871715"></a><a name="p381383871715"></a><a href="查询告警规则列表.md">查询告警规则列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="p19813338201719"><a name="p19813338201719"></a><a name="p19813338201719"></a>查询系统当前告警规则列表。</p>
</td>
</tr>
<tr id="row1459164191718"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p445914191711"><a name="p445914191711"></a><a name="p445914191711"></a><a href="查询单条告警规则信息.md">查询单条告警规则信息</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p84611241181719"><a name="p84611241181719"></a><a name="p84611241181719"></a>根据告警ID查询告警规则信息。</p>
</td>
</tr>
<tr id="row1987820263297"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p8939172693215"><a name="p8939172693215"></a><a name="p8939172693215"></a><a href="启停告警规则.md">启停告警规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p86434284717"><a name="p86434284717"></a><a name="p86434284717"></a>根据告警ID启动或停止一条告警规则。</p>
</td>
</tr>
<tr id="row699074913185"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p199904498185"><a name="p199904498185"></a><a name="p199904498185"></a><a href="删除告警规则.md">删除告警规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p129901149151811"><a name="p129901149151811"></a><a name="p129901149151811"></a>根据告警ID删除一条告警规则。</p>
</td>
</tr>
<tr id="row12930105213186"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p12930175291816"><a name="p12930175291816"></a><a name="p12930175291816"></a><a href="创建告警规则.md">创建告警规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p129301052201813"><a name="p129301052201813"></a><a name="p129301052201813"></a>为系统当前的指标创建一条告警规则。</p>
</td>
</tr>
<tr id="row87746166614"><td class="cellrowborder" rowspan="4" valign="top" headers="mcps1.2.5.1.1 "><p id="p3606185844111"><a name="p3606185844111"></a><a name="p3606185844111"></a>监控数据管理</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p197741716567"><a name="p197741716567"></a><a name="p197741716567"></a><a href="查询监控数据.md">查询监控数据</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="p1477491610610"><a name="p1477491610610"></a><a name="p1477491610610"></a>查询指定时间范围指定指标的指定粒度的监控数据。</p>
</td>
</tr>
<tr id="row546063614192"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p19460636111913"><a name="p19460636111913"></a><a name="p19460636111913"></a><a href="添加监控数据.md">添加监控数据</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p1460236141919"><a name="p1460236141919"></a><a name="p1460236141919"></a>添加一条或多条指标监控数据。</p>
</td>
</tr>
<tr id="row122451939181915"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p1224523918198"><a name="p1224523918198"></a><a name="p1224523918198"></a><a href="批量查询监控数据.md">批量查询监控数据</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p15247113920190"><a name="p15247113920190"></a><a name="p15247113920190"></a>批量查询指定时间范围内指定指标的指定粒度的监控数据，目前最多支持10指标的批量查询。</p>
</td>
</tr>
<tr id="row10406172419614"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p940819240616"><a name="p940819240616"></a><a name="p940819240616"></a><a href="查询主机配置数据.md">查询主机配置数据</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p17408124564"><a name="p17408124564"></a><a name="p17408124564"></a>查询指定时间范围指定事件类型的主机配置数据，可以通过参数指定需要查询的数据维度。</p>
</td>
</tr>
<tr id="row816313459617"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p156748714214"><a name="p156748714214"></a><a name="p156748714214"></a>配额管理</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p375310191202"><a name="p375310191202"></a><a name="p375310191202"></a><a href="查询配额.md">查询配额</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="p7163194516616"><a name="p7163194516616"></a><a name="p7163194516616"></a>通过该接口可以查询告警规则配额。</p>
</td>
</tr>
<tr id="row132213492619"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p54751209429"><a name="p54751209429"></a><a name="p54751209429"></a>事件监控</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p9936130314"><a name="p9936130314"></a><a name="p9936130314"></a><a href="上报事件.md">上报事件</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="p15221849464"><a name="p15221849464"></a><a name="p15221849464"></a>通过该接口上报自定义事件。</p>
</td>
</tr>
</tbody>
</table>

