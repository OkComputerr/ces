# API网关监控指标说明<a name="ZH-CN_TOPIC_0084594894"></a>

## 功能说明<a name="section59820001153251"></a>

本节定义了API网关上报云监控的监控指标的命名空间，监控指标列表和维度定义，用户可以通过云监控提供的API接口来检索API网关产生的监控指标和告警信息。

## 命名空间<a name="section55128484153251"></a>

SYS.APIG

## 监控指标<a name="section57564324153251"></a>

<a name="table32198700153251"></a>
<table><thead align="left"><tr id="row43554686153251"><th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.1.6.1.1"><p id="p38268712153251"><a name="p38268712153251"></a><a name="p38268712153251"></a>指标</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.1.6.1.2"><p id="p12757995153251"><a name="p12757995153251"></a><a name="p12757995153251"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="31.546845315468452%" id="mcps1.1.6.1.3"><p id="p26764654153251"><a name="p26764654153251"></a><a name="p26764654153251"></a>含义</p>
</th>
<th class="cellrowborder" valign="top" width="15.388461153884613%" id="mcps1.1.6.1.4"><p id="p20453337153251"><a name="p20453337153251"></a><a name="p20453337153251"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.1.6.1.5"><p id="p46107605153251"><a name="p46107605153251"></a><a name="p46107605153251"></a>测量对象</p>
</th>
</tr>
</thead>
<tbody><tr id="row43728521153251"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.1.6.1.1 "><p id="p153107221155"><a name="p153107221155"></a><a name="p153107221155"></a>req_count</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.1.6.1.2 "><p id="p88431656037"><a name="p88431656037"></a><a name="p88431656037"></a>接口调用次数</p>
</td>
<td class="cellrowborder" valign="top" width="31.546845315468452%" headers="mcps1.1.6.1.3 "><p id="p876610401528"><a name="p876610401528"></a><a name="p876610401528"></a>该指标用于统计测量api接口调用次数。以次/分钟为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="15.388461153884613%" headers="mcps1.1.6.1.4 "><p id="p7768340322"><a name="p7768340322"></a><a name="p7768340322"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.1.6.1.5 "><p id="p176817408219"><a name="p176817408219"></a><a name="p176817408219"></a>api接口</p>
</td>
</tr>
<tr id="row15045394153251"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.1.6.1.1 "><p id="p031019221852"><a name="p031019221852"></a><a name="p031019221852"></a>req_count_2xx</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.1.6.1.2 "><p id="p78431356137"><a name="p78431356137"></a><a name="p78431356137"></a>2xx调用次数</p>
</td>
<td class="cellrowborder" valign="top" width="31.546845315468452%" headers="mcps1.1.6.1.3 "><p id="p0773154018214"><a name="p0773154018214"></a><a name="p0773154018214"></a>该指标用于统计测量api接口调用2xx的次数。以次/分钟为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="15.388461153884613%" headers="mcps1.1.6.1.4 "><p id="p167747401220"><a name="p167747401220"></a><a name="p167747401220"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.1.6.1.5 "><p id="p177514403211"><a name="p177514403211"></a><a name="p177514403211"></a>api接口</p>
</td>
</tr>
<tr id="row39987979153251"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.1.6.1.1 "><p id="p103101522251"><a name="p103101522251"></a><a name="p103101522251"></a>req_count_4xx</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.1.6.1.2 "><p id="p48438562311"><a name="p48438562311"></a><a name="p48438562311"></a>4xx异常次数</p>
</td>
<td class="cellrowborder" valign="top" width="31.546845315468452%" headers="mcps1.1.6.1.3 "><p id="p177773407215"><a name="p177773407215"></a><a name="p177773407215"></a>该指标用于统计测量api接口返回4xx错误的次数。以次/分钟为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="15.388461153884613%" headers="mcps1.1.6.1.4 "><p id="p1596434112115"><a name="p1596434112115"></a><a name="p1596434112115"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.1.6.1.5 "><p id="p10779174012211"><a name="p10779174012211"></a><a name="p10779174012211"></a>api接口</p>
</td>
</tr>
<tr id="row27949047153251"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.1.6.1.1 "><p id="p183107221520"><a name="p183107221520"></a><a name="p183107221520"></a>req_count_5xx</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.1.6.1.2 "><p id="p1784313568315"><a name="p1784313568315"></a><a name="p1784313568315"></a>5xx异常次数</p>
</td>
<td class="cellrowborder" valign="top" width="31.546845315468452%" headers="mcps1.1.6.1.3 "><p id="p64751505153251"><a name="p64751505153251"></a><a name="p64751505153251"></a>该指标用于统计测量api接口返回5xx错误的次数。以次/分钟为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="15.388461153884613%" headers="mcps1.1.6.1.4 "><p id="p7966114117119"><a name="p7966114117119"></a><a name="p7966114117119"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.1.6.1.5 "><p id="p35516633153251"><a name="p35516633153251"></a><a name="p35516633153251"></a>api接口</p>
</td>
</tr>
<tr id="row51214241153251"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.1.6.1.1 "><p id="p631112211511"><a name="p631112211511"></a><a name="p631112211511"></a>avg_latency</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.1.6.1.2 "><p id="p1184318561930"><a name="p1184318561930"></a><a name="p1184318561930"></a>平均延迟毫秒数</p>
</td>
<td class="cellrowborder" valign="top" width="31.546845315468452%" headers="mcps1.1.6.1.3 "><p id="p5637610153251"><a name="p5637610153251"></a><a name="p5637610153251"></a>该指标用于统计测量api接口平均响应延时时间。以毫秒为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="15.388461153884613%" headers="mcps1.1.6.1.4 "><p id="p894334911113"><a name="p894334911113"></a><a name="p894334911113"></a>≥ 0 ms</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.1.6.1.5 "><p id="p11378541153251"><a name="p11378541153251"></a><a name="p11378541153251"></a>api接口</p>
</td>
</tr>
<tr id="row35298012153251"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.1.6.1.1 "><p id="p13311142212510"><a name="p13311142212510"></a><a name="p13311142212510"></a>max_latency</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.1.6.1.2 "><p id="p158433561032"><a name="p158433561032"></a><a name="p158433561032"></a>最大延迟毫秒数</p>
</td>
<td class="cellrowborder" valign="top" width="31.546845315468452%" headers="mcps1.1.6.1.3 "><p id="p4509250153251"><a name="p4509250153251"></a><a name="p4509250153251"></a>该指标用于统计测量api接口最大响应延时时间。以毫秒为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="15.388461153884613%" headers="mcps1.1.6.1.4 "><p id="p10944249101119"><a name="p10944249101119"></a><a name="p10944249101119"></a>≥ 0 ms</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.1.6.1.5 "><p id="p57295253153251"><a name="p57295253153251"></a><a name="p57295253153251"></a>api接口</p>
</td>
</tr>
<tr id="row480532827"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.1.6.1.1 "><p id="p63112228511"><a name="p63112228511"></a><a name="p63112228511"></a>output_throughput</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.1.6.1.2 "><p id="p15843856233"><a name="p15843856233"></a><a name="p15843856233"></a>返回流量</p>
</td>
<td class="cellrowborder" valign="top" width="31.546845315468452%" headers="mcps1.1.6.1.3 "><p id="p13551332727"><a name="p13551332727"></a><a name="p13551332727"></a>该指标用于统计测量api接口返回流量。以字节为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="15.388461153884613%" headers="mcps1.1.6.1.4 "><p id="p189465496111"><a name="p189465496111"></a><a name="p189465496111"></a>≥ 0 byte</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.1.6.1.5 "><p id="p55713215214"><a name="p55713215214"></a><a name="p55713215214"></a>api接口</p>
</td>
</tr>
<tr id="row11801632823"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.1.6.1.1 "><p id="p133111622655"><a name="p133111622655"></a><a name="p133111622655"></a>input_throughput</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.1.6.1.2 "><p id="p78451256936"><a name="p78451256936"></a><a name="p78451256936"></a>请求流量</p>
</td>
<td class="cellrowborder" valign="top" width="31.546845315468452%" headers="mcps1.1.6.1.3 "><p id="p146116323213"><a name="p146116323213"></a><a name="p146116323213"></a>该指标用于统计测量api接口请求流量。以字节为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="15.388461153884613%" headers="mcps1.1.6.1.4 "><p id="p2948154917114"><a name="p2948154917114"></a><a name="p2948154917114"></a>≥ 0 byte</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.1.6.1.5 "><p id="p36312327212"><a name="p36312327212"></a><a name="p36312327212"></a>api接口</p>
</td>
</tr>
<tr id="row117717327218"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.1.6.1.1 "><p id="p23111922050"><a name="p23111922050"></a><a name="p23111922050"></a>req_count_error</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.1.6.1.2 "><p id="p1184595615310"><a name="p1184595615310"></a><a name="p1184595615310"></a>总的错误次数</p>
</td>
<td class="cellrowborder" valign="top" width="31.546845315468452%" headers="mcps1.1.6.1.3 "><p id="p96623219215"><a name="p96623219215"></a><a name="p96623219215"></a>该指标用于统计测量api接口总的错误次数，以次/分钟为单位。</p>
</td>
<td class="cellrowborder" valign="top" width="15.388461153884613%" headers="mcps1.1.6.1.4 "><p id="p1122145541119"><a name="p1122145541119"></a><a name="p1122145541119"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.1.6.1.5 "><p id="p1968532728"><a name="p1968532728"></a><a name="p1968532728"></a>api接口</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="section45895235153251"></a>

<a name="table26526577153251"></a>
<table><thead align="left"><tr id="row46969777153251"><th class="cellrowborder" valign="top" width="40.400000000000006%" id="mcps1.1.3.1.1"><p id="p46455583153251"><a name="p46455583153251"></a><a name="p46455583153251"></a>Key</p>
</th>
<th class="cellrowborder" valign="top" width="59.599999999999994%" id="mcps1.1.3.1.2"><p id="p4805882153251"><a name="p4805882153251"></a><a name="p4805882153251"></a>Value</p>
</th>
</tr>
</thead>
<tbody><tr id="row53732137153251"><td class="cellrowborder" valign="top" width="40.400000000000006%" headers="mcps1.1.3.1.1 "><p id="p57335829153251"><a name="p57335829153251"></a><a name="p57335829153251"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="59.599999999999994%" headers="mcps1.1.3.1.2 "><p id="p13690533153251"><a name="p13690533153251"></a><a name="p13690533153251"></a>api接口</p>
</td>
</tr>
</tbody>
</table>

