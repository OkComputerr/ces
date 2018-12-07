# Web应用防火墙的监控指标<a name="ZH-CN_TOPIC_0084572267"></a>

**表 1**  Web应用防火墙支持的监控指标

<a name="table539544351613"></a>
<table><thead align="left"><tr id="zh-cn_topic_0015479905_row14798174974914"><th class="cellrowborder" valign="top" width="23%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0015479905_p1798349184915"><a name="zh-cn_topic_0015479905_p1798349184915"></a><a name="zh-cn_topic_0015479905_p1798349184915"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="32%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0015479905_p10798114964914"><a name="zh-cn_topic_0015479905_p10798114964914"></a><a name="zh-cn_topic_0015479905_p10798114964914"></a>指标含义</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0015479905_p1879884912490"><a name="zh-cn_topic_0015479905_p1879884912490"></a><a name="zh-cn_topic_0015479905_p1879884912490"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0015479905_p14798049174918"><a name="zh-cn_topic_0015479905_p14798049174918"></a><a name="zh-cn_topic_0015479905_p14798049174918"></a>测量对象</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0015479905_p1611711113212"><a name="zh-cn_topic_0015479905_p1611711113212"></a><a name="zh-cn_topic_0015479905_p1611711113212"></a>监控周期（原始指标）</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0015479905_row1279820497494"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p17983496496"><a name="zh-cn_topic_0015479905_p17983496496"></a><a name="zh-cn_topic_0015479905_p17983496496"></a>SQL注入告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p157983498490"><a name="zh-cn_topic_0015479905_p157983498490"></a><a name="zh-cn_topic_0015479905_p157983498490"></a>该指标用于统计测量对象的SQL注入告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p079844910498"><a name="zh-cn_topic_0015479905_p079844910498"></a><a name="zh-cn_topic_0015479905_p079844910498"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p1879874974916"><a name="zh-cn_topic_0015479905_p1879874974916"></a><a name="zh-cn_topic_0015479905_p1879874974916"></a>弹性云服务器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p1411911103212"><a name="zh-cn_topic_0015479905_p1411911103212"></a><a name="zh-cn_topic_0015479905_p1411911103212"></a>4分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row1879824912492"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p57981149154912"><a name="zh-cn_topic_0015479905_p57981149154912"></a><a name="zh-cn_topic_0015479905_p57981149154912"></a>XSS跨站脚本漏洞告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p11798174912492"><a name="zh-cn_topic_0015479905_p11798174912492"></a><a name="zh-cn_topic_0015479905_p11798174912492"></a>该指标用于统计测量对象的XSS跨站脚本漏洞告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p4798114911493"><a name="zh-cn_topic_0015479905_p4798114911493"></a><a name="zh-cn_topic_0015479905_p4798114911493"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p117987495495"><a name="zh-cn_topic_0015479905_p117987495495"></a><a name="zh-cn_topic_0015479905_p117987495495"></a>弹性云服务器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p1311611203217"><a name="zh-cn_topic_0015479905_p1311611203217"></a><a name="zh-cn_topic_0015479905_p1311611203217"></a>4分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row157989497491"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p127981349174913"><a name="zh-cn_topic_0015479905_p127981349174913"></a><a name="zh-cn_topic_0015479905_p127981349174913"></a>Webshell上传告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p1579844964916"><a name="zh-cn_topic_0015479905_p1579844964916"></a><a name="zh-cn_topic_0015479905_p1579844964916"></a>该指标用于统计测量对象的Webshell上传告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p1579818492498"><a name="zh-cn_topic_0015479905_p1579818492498"></a><a name="zh-cn_topic_0015479905_p1579818492498"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p14798104910491"><a name="zh-cn_topic_0015479905_p14798104910491"></a><a name="zh-cn_topic_0015479905_p14798104910491"></a>弹性云服务器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p201101113328"><a name="zh-cn_topic_0015479905_p201101113328"></a><a name="zh-cn_topic_0015479905_p201101113328"></a>4分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row67982049174911"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p1179815498493"><a name="zh-cn_topic_0015479905_p1179815498493"></a><a name="zh-cn_topic_0015479905_p1179815498493"></a>盗链告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p8798449124920"><a name="zh-cn_topic_0015479905_p8798449124920"></a><a name="zh-cn_topic_0015479905_p8798449124920"></a>该指标用于统计测量对象的盗链告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p57985494495"><a name="zh-cn_topic_0015479905_p57985494495"></a><a name="zh-cn_topic_0015479905_p57985494495"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p1179894919494"><a name="zh-cn_topic_0015479905_p1179894919494"></a><a name="zh-cn_topic_0015479905_p1179894919494"></a>弹性云服务器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p13119111326"><a name="zh-cn_topic_0015479905_p13119111326"></a><a name="zh-cn_topic_0015479905_p13119111326"></a>4分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row18798184916491"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p19798134974914"><a name="zh-cn_topic_0015479905_p19798134974914"></a><a name="zh-cn_topic_0015479905_p19798134974914"></a>IP黑名单告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p9798124913499"><a name="zh-cn_topic_0015479905_p9798124913499"></a><a name="zh-cn_topic_0015479905_p9798124913499"></a>该指标用于统计测量对象的IP黑名单告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p17981949124916"><a name="zh-cn_topic_0015479905_p17981949124916"></a><a name="zh-cn_topic_0015479905_p17981949124916"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p16798124919498"><a name="zh-cn_topic_0015479905_p16798124919498"></a><a name="zh-cn_topic_0015479905_p16798124919498"></a>弹性云服务器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p4181119327"><a name="zh-cn_topic_0015479905_p4181119327"></a><a name="zh-cn_topic_0015479905_p4181119327"></a>4分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row47988492495"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p87981749134915"><a name="zh-cn_topic_0015479905_p87981749134915"></a><a name="zh-cn_topic_0015479905_p87981749134915"></a>IP白名单告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p137981449104910"><a name="zh-cn_topic_0015479905_p137981449104910"></a><a name="zh-cn_topic_0015479905_p137981449104910"></a>该指标用于统计测量对象的IP白名单告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p1779815495498"><a name="zh-cn_topic_0015479905_p1779815495498"></a><a name="zh-cn_topic_0015479905_p1779815495498"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p107981049114910"><a name="zh-cn_topic_0015479905_p107981049114910"></a><a name="zh-cn_topic_0015479905_p107981049114910"></a>弹性云服务器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p5161183213"><a name="zh-cn_topic_0015479905_p5161183213"></a><a name="zh-cn_topic_0015479905_p5161183213"></a>4分钟</p>
</td>
</tr>
</tbody>
</table>

