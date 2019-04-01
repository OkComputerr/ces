# Web应用防火墙监控指标说明<a name="ZH-CN_TOPIC_0077629995"></a>

## 功能说明<a name="zh-cn_topic_0067114431_section7818464131458"></a>

本节定义了Web应用防火墙服务上报云监控指标的命名空间，监控指标列表和维度定义，用户可以通过云监控服务提供的API接口来检索Web应用防火墙服务产生的监控指标和告警信息。

## 命名空间<a name="zh-cn_topic_0067114431_section63878810131529"></a>

SYS.WAF

## 监控指标<a name="zh-cn_topic_0067114431_section64753703131557"></a>

<a name="zh-cn_topic_0067114431_table5331155094045"></a>
<table><thead align="left"><tr id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_row4079778316522"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.6.1.1"><p id="zh-cn_topic_0067114431_p1784101911244"><a name="zh-cn_topic_0067114431_p1784101911244"></a><a name="zh-cn_topic_0067114431_p1784101911244"></a>指标</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.2"><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5604842816535"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5604842816535"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5604842816535"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="32%" id="mcps1.1.6.1.3"><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5711500816535"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5711500816535"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5711500816535"></a>指标含义</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.1.6.1.4"><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2934585916535"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2934585916535"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2934585916535"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.1.6.1.5"><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5251292716535"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5251292716535"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5251292716535"></a>测量对象</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_row6652713516522"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0067114431_p22890152112437"><a name="zh-cn_topic_0067114431_p22890152112437"></a><a name="zh-cn_topic_0067114431_p22890152112437"></a>sql_injection_alarms</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p156401051664"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p156401051664"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p156401051664"></a>SQL注入告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p588890221664"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p588890221664"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p588890221664"></a>该指标用于统计测量对象的SQL注入告警个数。</p>
<p id="p3272446351"><a name="p3272446351"></a><a name="p3272446351"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p52815001664"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p52815001664"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p52815001664"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p251483301664"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p251483301664"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p251483301664"></a>弹性云服务器</p>
</td>
</tr>
<tr id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_row99919716522"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0067114431_p43922867112437"><a name="zh-cn_topic_0067114431_p43922867112437"></a><a name="zh-cn_topic_0067114431_p43922867112437"></a>xss_vulnerability_alarms</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1963431016635"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1963431016635"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1963431016635"></a>XSS跨站脚本漏洞告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4687527316635"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4687527316635"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4687527316635"></a>该指标用于统计测量对象的XSS跨站脚本漏洞告警个数。</p>
<p id="p868417617351"><a name="p868417617351"></a><a name="p868417617351"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p3880077716635"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p3880077716635"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p3880077716635"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5585521316635"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5585521316635"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5585521316635"></a>弹性云服务器</p>
</td>
</tr>
<tr id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_row2063427516522"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0067114431_p8842463112437"><a name="zh-cn_topic_0067114431_p8842463112437"></a><a name="zh-cn_topic_0067114431_p8842463112437"></a>webshell_upload_alarms</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2342649116641"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2342649116641"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2342649116641"></a>Webshell上传告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1849760416641"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1849760416641"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1849760416641"></a>该指标用于统计测量对象的Webshell上传告警个数。</p>
<p id="p12519161043518"><a name="p12519161043518"></a><a name="p12519161043518"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2191095416641"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2191095416641"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2191095416641"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2995682016641"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2995682016641"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p2995682016641"></a>弹性云服务器</p>
</td>
</tr>
<tr id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_row4566152016522"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0067114431_p3704709112437"><a name="zh-cn_topic_0067114431_p3704709112437"></a><a name="zh-cn_topic_0067114431_p3704709112437"></a>link_theft_alarms</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p3566310716653"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p3566310716653"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p3566310716653"></a>盗链告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p303056016653"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p303056016653"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p303056016653"></a>该指标用于统计测量对象的盗链告警个数。</p>
<p id="p151261113133515"><a name="p151261113133515"></a><a name="p151261113133515"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4414882616653"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4414882616653"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4414882616653"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1928514416653"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1928514416653"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1928514416653"></a>弹性云服务器</p>
</td>
</tr>
<tr id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_row2447886316522"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0067114431_p16378826112437"><a name="zh-cn_topic_0067114431_p16378826112437"></a><a name="zh-cn_topic_0067114431_p16378826112437"></a>ip_address_blacklist_alarms</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p333201141672"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p333201141672"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p333201141672"></a>IP黑名单告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p145747141672"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p145747141672"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p145747141672"></a>该指标用于统计测量对象的IP黑名单告警个数。</p>
<p id="p59815152355"><a name="p59815152355"></a><a name="p59815152355"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p397011991672"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p397011991672"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p397011991672"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p616805361672"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p616805361672"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p616805361672"></a>弹性云服务器</p>
</td>
</tr>
<tr id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_row2526728016522"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0067114431_p61895512112437"><a name="zh-cn_topic_0067114431_p61895512112437"></a><a name="zh-cn_topic_0067114431_p61895512112437"></a>ip_address_whitelist_alarms</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1805936716712"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1805936716712"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p1805936716712"></a>IP白名单告警个数</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5352264316712"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5352264316712"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p5352264316712"></a>该指标用于统计测量对象的IP白名单告警个数。</p>
<p id="p4848917193513"><a name="p4848917193513"></a><a name="p4848917193513"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4036686016712"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4036686016712"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4036686016712"></a>≥0 count</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4849023316712"><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4849023316712"></a><a name="zh-cn_topic_0067114431_zh-cn_topic_0015479905_p4849023316712"></a>弹性云服务器</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="zh-cn_topic_0067114431_section63551882131628"></a>

<a name="zh-cn_topic_0067114431_table2768457312211"></a>
<table><thead align="left"><tr id="zh-cn_topic_0067114431_row4156438612211"><th class="cellrowborder" valign="top" width="46.06%" id="mcps1.1.3.1.1"><p id="zh-cn_topic_0067114431_p1127207512211"><a name="zh-cn_topic_0067114431_p1127207512211"></a><a name="zh-cn_topic_0067114431_p1127207512211"></a><strong id="zh-cn_topic_0067114431_b3433981112211"><a name="zh-cn_topic_0067114431_b3433981112211"></a><a name="zh-cn_topic_0067114431_b3433981112211"></a>Key</strong></p>
</th>
<th class="cellrowborder" valign="top" width="53.94%" id="mcps1.1.3.1.2"><p id="zh-cn_topic_0067114431_p3006127912211"><a name="zh-cn_topic_0067114431_p3006127912211"></a><a name="zh-cn_topic_0067114431_p3006127912211"></a><strong id="zh-cn_topic_0067114431_b211606212211"><a name="zh-cn_topic_0067114431_b211606212211"></a><a name="zh-cn_topic_0067114431_b211606212211"></a>Value</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0067114431_row1904456012211"><td class="cellrowborder" valign="top" width="46.06%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0067114431_p6621443012211"><a name="zh-cn_topic_0067114431_p6621443012211"></a><a name="zh-cn_topic_0067114431_p6621443012211"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="53.94%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0067114431_p6176862412211"><a name="zh-cn_topic_0067114431_p6176862412211"></a><a name="zh-cn_topic_0067114431_p6176862412211"></a>弹性云服务器实例ID</p>
</td>
</tr>
</tbody>
</table>

