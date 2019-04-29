# 弹性公网IP和带宽监控指标说明<a name="ZH-CN_TOPIC_0024746310"></a>

## 功能说明<a name="zh-cn_topic_0024607920_section45043704193247"></a>

本节定义了弹性公网IP和带宽上报云监控的监控指标的命名空间，监控指标列表和维度定义，用户可以通过云监控提供的API接口来检索弹性公网IP和带宽产生的监控指标和告警信息。

## 命名空间<a name="zh-cn_topic_0024607920_section20626347193247"></a>

SYS.VPC

## 监控指标<a name="zh-cn_topic_0024607920_section4222089193247"></a>

**表 1**  弹性公网IP和带宽支持的监控指标

<a name="zh-cn_topic_0024607920_table6444895193247"></a>
<table><thead align="left"><tr id="zh-cn_topic_0024607920_row17328334193247"><th class="cellrowborder" valign="top" width="19.000000000000004%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0024607920_p61417783193247"><a name="zh-cn_topic_0024607920_p61417783193247"></a><a name="zh-cn_topic_0024607920_p61417783193247"></a>指标</p>
</th>
<th class="cellrowborder" valign="top" width="16.000000000000004%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0024607920_p8784488193247"><a name="zh-cn_topic_0024607920_p8784488193247"></a><a name="zh-cn_topic_0024607920_p8784488193247"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="29.000000000000004%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0024607920_p40454922193247"><a name="zh-cn_topic_0024607920_p40454922193247"></a><a name="zh-cn_topic_0024607920_p40454922193247"></a>含义</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000004%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0024607920_p55623236193247"><a name="zh-cn_topic_0024607920_p55623236193247"></a><a name="zh-cn_topic_0024607920_p55623236193247"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="22.000000000000004%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0024607920_p9188287193247"><a name="zh-cn_topic_0024607920_p9188287193247"></a><a name="zh-cn_topic_0024607920_p9188287193247"></a>测试对象</p>
</th>
</tr>
</thead>
<tbody><tr id="row176441730192910"><td class="cellrowborder" valign="top" width="19.000000000000004%" headers="mcps1.2.6.1.1 "><p id="p168131935132918"><a name="p168131935132918"></a><a name="p168131935132918"></a>up_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="16.000000000000004%" headers="mcps1.2.6.1.2 "><p id="p1981512351293"><a name="p1981512351293"></a><a name="p1981512351293"></a>出网带宽（已废弃）</p>
</td>
<td class="cellrowborder" valign="top" width="29.000000000000004%" headers="mcps1.2.6.1.3 "><p id="p8483191441612"><a name="p8483191441612"></a><a name="p8483191441612"></a>该指标用于统计测试对象出云平台的网络速度（原指标为上行带宽）。</p>
<p id="p1738001814508"><a name="p1738001814508"></a><a name="p1738001814508"></a>该指标用于华北-北京一、华东-上海二、华南-广州。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000004%" headers="mcps1.2.6.1.4 "><p id="p940181671414"><a name="p940181671414"></a><a name="p940181671414"></a>≥ 0 bytes/s</p>
</td>
<td class="cellrowborder" valign="top" width="22.000000000000004%" headers="mcps1.2.6.1.5 "><p id="p14820235172920"><a name="p14820235172920"></a><a name="p14820235172920"></a>带宽或弹性公网IP。</p>
</td>
</tr>
<tr id="row1757363418295"><td class="cellrowborder" valign="top" width="19.000000000000004%" headers="mcps1.2.6.1.1 "><p id="p9824635142912"><a name="p9824635142912"></a><a name="p9824635142912"></a>down_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="16.000000000000004%" headers="mcps1.2.6.1.2 "><p id="p19826935192917"><a name="p19826935192917"></a><a name="p19826935192917"></a>入网带宽（已废弃）</p>
</td>
<td class="cellrowborder" valign="top" width="29.000000000000004%" headers="mcps1.2.6.1.3 "><p id="p1143816191415"><a name="p1143816191415"></a><a name="p1143816191415"></a>该指标用于统计测试对象入云平台的网络速度（原指标为下行带宽）。</p>
<p id="p2053915114"><a name="p2053915114"></a><a name="p2053915114"></a>该指标用于华北-北京一、华东-上海二、华南-广州。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000004%" headers="mcps1.2.6.1.4 "><p id="p20441016151411"><a name="p20441016151411"></a><a name="p20441016151411"></a>≥ 0 bytes/s</p>
</td>
<td class="cellrowborder" valign="top" width="22.000000000000004%" headers="mcps1.2.6.1.5 "><p id="p1183233552919"><a name="p1183233552919"></a><a name="p1183233552919"></a>带宽或弹性公网IP。</p>
</td>
</tr>
<tr id="row14752162934912"><td class="cellrowborder" valign="top" width="19.000000000000004%" headers="mcps1.2.6.1.1 "><p id="p143066346498"><a name="p143066346498"></a><a name="p143066346498"></a>up_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="16.000000000000004%" headers="mcps1.2.6.1.2 "><p id="p20307934134916"><a name="p20307934134916"></a><a name="p20307934134916"></a>出网带宽</p>
</td>
<td class="cellrowborder" valign="top" width="29.000000000000004%" headers="mcps1.2.6.1.3 "><p id="p3310163417492"><a name="p3310163417492"></a><a name="p3310163417492"></a>该指标用于统计测试对象出云平台的网络速度（原指标为上行带宽）。</p>
<p id="p20553011105114"><a name="p20553011105114"></a><a name="p20553011105114"></a>该指标用于亚太-香港、亚太-曼谷。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000004%" headers="mcps1.2.6.1.4 "><p id="p831119344492"><a name="p831119344492"></a><a name="p831119344492"></a>≥ 0 bytes/s</p>
</td>
<td class="cellrowborder" valign="top" width="22.000000000000004%" headers="mcps1.2.6.1.5 "><p id="p10315203434914"><a name="p10315203434914"></a><a name="p10315203434914"></a>带宽或弹性公网IP。</p>
</td>
</tr>
<tr id="row155601329495"><td class="cellrowborder" valign="top" width="19.000000000000004%" headers="mcps1.2.6.1.1 "><p id="p19318434184914"><a name="p19318434184914"></a><a name="p19318434184914"></a>down_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="16.000000000000004%" headers="mcps1.2.6.1.2 "><p id="p832093410495"><a name="p832093410495"></a><a name="p832093410495"></a>入网带宽</p>
</td>
<td class="cellrowborder" valign="top" width="29.000000000000004%" headers="mcps1.2.6.1.3 "><p id="p33221434174915"><a name="p33221434174915"></a><a name="p33221434174915"></a>该指标用于统计测试对象入云平台的网络速度（原指标为下行带宽）。</p>
<p id="p12804523145113"><a name="p12804523145113"></a><a name="p12804523145113"></a>该指标用于亚太-香港、亚太-曼谷。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000004%" headers="mcps1.2.6.1.4 "><p id="p13323183464914"><a name="p13323183464914"></a><a name="p13323183464914"></a>≥ 0 bytes/s</p>
</td>
<td class="cellrowborder" valign="top" width="22.000000000000004%" headers="mcps1.2.6.1.5 "><p id="p532583474919"><a name="p532583474919"></a><a name="p532583474919"></a>带宽或弹性公网IP。</p>
</td>
</tr>
<tr id="zh-cn_topic_0024607920_row173875718321"><td class="cellrowborder" valign="top" width="19.000000000000004%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0024607920_p131326819339"><a name="zh-cn_topic_0024607920_p131326819339"></a><a name="zh-cn_topic_0024607920_p131326819339"></a>upstream_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="16.000000000000004%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0024607920_p7133182333"><a name="zh-cn_topic_0024607920_p7133182333"></a><a name="zh-cn_topic_0024607920_p7133182333"></a>出网带宽</p>
</td>
<td class="cellrowborder" valign="top" width="29.000000000000004%" headers="mcps1.2.6.1.3 "><p id="p179215408321"><a name="p179215408321"></a><a name="p179215408321"></a>该指标用于统计测试对象出云平台的网络速度（原指标为上行带宽）。</p>
<p id="p15604546145113"><a name="p15604546145113"></a><a name="p15604546145113"></a>该指标用于华北-北京一、华东-上海二、华南-广州。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000004%" headers="mcps1.2.6.1.4 "><p id="p16856133111520"><a name="p16856133111520"></a><a name="p16856133111520"></a>≥ 0 bits/s</p>
</td>
<td class="cellrowborder" valign="top" width="22.000000000000004%" headers="mcps1.2.6.1.5 "><p id="p932911508322"><a name="p932911508322"></a><a name="p932911508322"></a>带宽或弹性公网IP。</p>
</td>
</tr>
<tr id="zh-cn_topic_0024607920_row2515145493216"><td class="cellrowborder" valign="top" width="19.000000000000004%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0024607920_p131416813315"><a name="zh-cn_topic_0024607920_p131416813315"></a><a name="zh-cn_topic_0024607920_p131416813315"></a>downstream_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="16.000000000000004%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0024607920_p18143178133311"><a name="zh-cn_topic_0024607920_p18143178133311"></a><a name="zh-cn_topic_0024607920_p18143178133311"></a>入网带宽</p>
</td>
<td class="cellrowborder" valign="top" width="29.000000000000004%" headers="mcps1.2.6.1.3 "><p id="p14794440113211"><a name="p14794440113211"></a><a name="p14794440113211"></a>该指标用于统计测试对象入云平台的网络速度（原指标为下行带宽）。</p>
<p id="p189801749135116"><a name="p189801749135116"></a><a name="p189801749135116"></a>该指标用于华北-北京一、华东-上海二、华南-广州。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000004%" headers="mcps1.2.6.1.4 "><p id="p1785863115157"><a name="p1785863115157"></a><a name="p1785863115157"></a>≥ 0 bits/s</p>
</td>
<td class="cellrowborder" valign="top" width="22.000000000000004%" headers="mcps1.2.6.1.5 "><p id="p1033275011323"><a name="p1033275011323"></a><a name="p1033275011323"></a>带宽或弹性公网IP。</p>
</td>
</tr>
<tr id="row79444328013"><td class="cellrowborder" valign="top" width="19.000000000000004%" headers="mcps1.2.6.1.1 "><p id="p131111534104"><a name="p131111534104"></a><a name="p131111534104"></a>upstream_bandwidth_usage</p>
</td>
<td class="cellrowborder" valign="top" width="16.000000000000004%" headers="mcps1.2.6.1.2 "><p id="p1511110341407"><a name="p1511110341407"></a><a name="p1511110341407"></a>出网带宽使用率</p>
</td>
<td class="cellrowborder" valign="top" width="29.000000000000004%" headers="mcps1.2.6.1.3 "><p id="p11114123410010"><a name="p11114123410010"></a><a name="p11114123410010"></a>该指标用于统计测量对象出云平台的带宽使用率，以百分比为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000004%" headers="mcps1.2.6.1.4 "><p id="p14892155717598"><a name="p14892155717598"></a><a name="p14892155717598"></a>0-100%</p>
</td>
<td class="cellrowborder" valign="top" width="22.000000000000004%" headers="mcps1.2.6.1.5 "><p id="p1711913341012"><a name="p1711913341012"></a><a name="p1711913341012"></a>带宽或弹性公网IP。</p>
</td>
</tr>
<tr id="row6251357113315"><td class="cellrowborder" valign="top" width="19.000000000000004%" headers="mcps1.2.6.1.1 "><p id="p199051635348"><a name="p199051635348"></a><a name="p199051635348"></a>up_stream</p>
</td>
<td class="cellrowborder" valign="top" width="16.000000000000004%" headers="mcps1.2.6.1.2 "><p id="p55042030141711"><a name="p55042030141711"></a><a name="p55042030141711"></a>出网流量</p>
</td>
<td class="cellrowborder" valign="top" width="29.000000000000004%" headers="mcps1.2.6.1.3 "><p id="p050623091713"><a name="p050623091713"></a><a name="p050623091713"></a>该指标用于统计测试对象出云平台的网络流量（原指标为上行流量）。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000004%" headers="mcps1.2.6.1.4 "><p id="p55084302174"><a name="p55084302174"></a><a name="p55084302174"></a>≥ 0 bytes</p>
</td>
<td class="cellrowborder" valign="top" width="22.000000000000004%" headers="mcps1.2.6.1.5 "><p id="p1275192733415"><a name="p1275192733415"></a><a name="p1275192733415"></a>带宽或弹性公网IP。</p>
</td>
</tr>
<tr id="row84711354143318"><td class="cellrowborder" valign="top" width="19.000000000000004%" headers="mcps1.2.6.1.1 "><p id="p29277317341"><a name="p29277317341"></a><a name="p29277317341"></a>down_stream</p>
</td>
<td class="cellrowborder" valign="top" width="16.000000000000004%" headers="mcps1.2.6.1.2 "><p id="p1451019302175"><a name="p1451019302175"></a><a name="p1451019302175"></a>入网流量</p>
</td>
<td class="cellrowborder" valign="top" width="29.000000000000004%" headers="mcps1.2.6.1.3 "><p id="p1051010308176"><a name="p1051010308176"></a><a name="p1051010308176"></a>该指标用于统计测试对象入云平台的网络流量（原指标为下行流量）。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000004%" headers="mcps1.2.6.1.4 "><p id="p15512163016174"><a name="p15512163016174"></a><a name="p15512163016174"></a>≥ 0 bytes</p>
</td>
<td class="cellrowborder" valign="top" width="22.000000000000004%" headers="mcps1.2.6.1.5 "><p id="p1977727183412"><a name="p1977727183412"></a><a name="p1977727183412"></a>带宽或弹性公网IP。</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="zh-cn_topic_0024607920_section27751125193247"></a>

<a name="zh-cn_topic_0024607920_table30802540193247"></a>
<table><thead align="left"><tr id="zh-cn_topic_0024607920_row7692483193247"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="zh-cn_topic_0024607920_p19111369193247"><a name="zh-cn_topic_0024607920_p19111369193247"></a><a name="zh-cn_topic_0024607920_p19111369193247"></a>Key</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="zh-cn_topic_0024607920_p4517093193247"><a name="zh-cn_topic_0024607920_p4517093193247"></a><a name="zh-cn_topic_0024607920_p4517093193247"></a>Value</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0024607920_row30340220193247"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0024607920_p41638776193247"><a name="zh-cn_topic_0024607920_p41638776193247"></a><a name="zh-cn_topic_0024607920_p41638776193247"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0024607920_p17297729193247"><a name="zh-cn_topic_0024607920_p17297729193247"></a><a name="zh-cn_topic_0024607920_p17297729193247"></a>弹性公网IP ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0024607920_row21461838193247"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0024607920_p60687284193247"><a name="zh-cn_topic_0024607920_p60687284193247"></a><a name="zh-cn_topic_0024607920_p60687284193247"></a>bandwidth_id</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0024607920_p16722971193247"><a name="zh-cn_topic_0024607920_p16722971193247"></a><a name="zh-cn_topic_0024607920_p16722971193247"></a>带宽ID</p>
</td>
</tr>
</tbody>
</table>

