# API网关的监控指标<a name="ZH-CN_TOPIC_0084799017"></a>

**表 1**  API网关支持的监控指标

<a name="table32198700153251"></a>
<table><thead align="left"><tr id="zh-cn_topic_0015479905_row898623515293"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0015479905_p19231136162915"><a name="zh-cn_topic_0015479905_p19231136162915"></a><a name="zh-cn_topic_0015479905_p19231136162915"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="34%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0015479905_p649936152915"><a name="zh-cn_topic_0015479905_p649936152915"></a><a name="zh-cn_topic_0015479905_p649936152915"></a>含义</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0015479905_p47610368292"><a name="zh-cn_topic_0015479905_p47610368292"></a><a name="zh-cn_topic_0015479905_p47610368292"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0015479905_p161115365291"><a name="zh-cn_topic_0015479905_p161115365291"></a><a name="zh-cn_topic_0015479905_p161115365291"></a>测量对象</p>
</th>
<th class="cellrowborder" valign="top" width="19%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0015479905_p484718584357"><a name="zh-cn_topic_0015479905_p484718584357"></a><a name="zh-cn_topic_0015479905_p484718584357"></a>监控周期（原始指标）</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0015479905_row19138436102915"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p88431656037"><a name="zh-cn_topic_0015479905_p88431656037"></a><a name="zh-cn_topic_0015479905_p88431656037"></a>接口调用次数</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p876610401528"><a name="zh-cn_topic_0015479905_p876610401528"></a><a name="zh-cn_topic_0015479905_p876610401528"></a>该指标用于统计测量api接口调用次数。</p>
<p id="zh-cn_topic_0015479905_p6727337205819"><a name="zh-cn_topic_0015479905_p6727337205819"></a><a name="zh-cn_topic_0015479905_p6727337205819"></a>单位：次/分钟</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p7768340322"><a name="zh-cn_topic_0015479905_p7768340322"></a><a name="zh-cn_topic_0015479905_p7768340322"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p176817408219"><a name="zh-cn_topic_0015479905_p176817408219"></a><a name="zh-cn_topic_0015479905_p176817408219"></a>api接口</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p384745823511"><a name="zh-cn_topic_0015479905_p384745823511"></a><a name="zh-cn_topic_0015479905_p384745823511"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row13275203618295"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p78431356137"><a name="zh-cn_topic_0015479905_p78431356137"></a><a name="zh-cn_topic_0015479905_p78431356137"></a>2xx调用次数</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p0773154018214"><a name="zh-cn_topic_0015479905_p0773154018214"></a><a name="zh-cn_topic_0015479905_p0773154018214"></a>该指标用于统计测量api接口调用2xx的次数。</p>
<p id="zh-cn_topic_0015479905_p143988157598"><a name="zh-cn_topic_0015479905_p143988157598"></a><a name="zh-cn_topic_0015479905_p143988157598"></a>单位：次/分钟</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p167747401220"><a name="zh-cn_topic_0015479905_p167747401220"></a><a name="zh-cn_topic_0015479905_p167747401220"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p177514403211"><a name="zh-cn_topic_0015479905_p177514403211"></a><a name="zh-cn_topic_0015479905_p177514403211"></a>api接口</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p384795883520"><a name="zh-cn_topic_0015479905_p384795883520"></a><a name="zh-cn_topic_0015479905_p384795883520"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row34147369296"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p48438562311"><a name="zh-cn_topic_0015479905_p48438562311"></a><a name="zh-cn_topic_0015479905_p48438562311"></a>4xx异常次数</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p177773407215"><a name="zh-cn_topic_0015479905_p177773407215"></a><a name="zh-cn_topic_0015479905_p177773407215"></a>该指标用于统计测量api接口返回4xx错误的次数。</p>
<p id="zh-cn_topic_0015479905_p1559892565916"><a name="zh-cn_topic_0015479905_p1559892565916"></a><a name="zh-cn_topic_0015479905_p1559892565916"></a>单位：次/分钟</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p1596434112115"><a name="zh-cn_topic_0015479905_p1596434112115"></a><a name="zh-cn_topic_0015479905_p1596434112115"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p10779174012211"><a name="zh-cn_topic_0015479905_p10779174012211"></a><a name="zh-cn_topic_0015479905_p10779174012211"></a>api接口</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p384795820353"><a name="zh-cn_topic_0015479905_p384795820353"></a><a name="zh-cn_topic_0015479905_p384795820353"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row8558163662916"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p1784313568315"><a name="zh-cn_topic_0015479905_p1784313568315"></a><a name="zh-cn_topic_0015479905_p1784313568315"></a>5xx异常次数</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p64751505153251"><a name="zh-cn_topic_0015479905_p64751505153251"></a><a name="zh-cn_topic_0015479905_p64751505153251"></a>该指标用于统计测量api接口返回5xx错误的次数。</p>
<p id="zh-cn_topic_0015479905_p5460315592"><a name="zh-cn_topic_0015479905_p5460315592"></a><a name="zh-cn_topic_0015479905_p5460315592"></a>单位：次/分钟</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p7966114117119"><a name="zh-cn_topic_0015479905_p7966114117119"></a><a name="zh-cn_topic_0015479905_p7966114117119"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p1967416363292"><a name="zh-cn_topic_0015479905_p1967416363292"></a><a name="zh-cn_topic_0015479905_p1967416363292"></a>api接口</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p939811573363"><a name="zh-cn_topic_0015479905_p939811573363"></a><a name="zh-cn_topic_0015479905_p939811573363"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row468583611297"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p1184318561930"><a name="zh-cn_topic_0015479905_p1184318561930"></a><a name="zh-cn_topic_0015479905_p1184318561930"></a>平均延迟毫秒数</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p868343918019"><a name="zh-cn_topic_0015479905_p868343918019"></a><a name="zh-cn_topic_0015479905_p868343918019"></a>该指标用于统计测量api接口平均响应延时时间。</p>
<p id="zh-cn_topic_0015479905_p5637610153251"><a name="zh-cn_topic_0015479905_p5637610153251"></a><a name="zh-cn_topic_0015479905_p5637610153251"></a>单位：毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p894334911113"><a name="zh-cn_topic_0015479905_p894334911113"></a><a name="zh-cn_topic_0015479905_p894334911113"></a>≥ 0 ms</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p8800336192920"><a name="zh-cn_topic_0015479905_p8800336192920"></a><a name="zh-cn_topic_0015479905_p8800336192920"></a>api接口</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p74419576364"><a name="zh-cn_topic_0015479905_p74419576364"></a><a name="zh-cn_topic_0015479905_p74419576364"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row98225366296"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p158433561032"><a name="zh-cn_topic_0015479905_p158433561032"></a><a name="zh-cn_topic_0015479905_p158433561032"></a>最大延迟毫秒数</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p4509250153251"><a name="zh-cn_topic_0015479905_p4509250153251"></a><a name="zh-cn_topic_0015479905_p4509250153251"></a>该指标用于统计测量api接口最大响应延时时间。</p>
<p id="zh-cn_topic_0015479905_p1641717181204"><a name="zh-cn_topic_0015479905_p1641717181204"></a><a name="zh-cn_topic_0015479905_p1641717181204"></a>单位：毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p10944249101119"><a name="zh-cn_topic_0015479905_p10944249101119"></a><a name="zh-cn_topic_0015479905_p10944249101119"></a>≥ 0 ms</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p293716368295"><a name="zh-cn_topic_0015479905_p293716368295"></a><a name="zh-cn_topic_0015479905_p293716368295"></a>api接口</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p19491957163613"><a name="zh-cn_topic_0015479905_p19491957163613"></a><a name="zh-cn_topic_0015479905_p19491957163613"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row480532827"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p15843856233"><a name="zh-cn_topic_0015479905_p15843856233"></a><a name="zh-cn_topic_0015479905_p15843856233"></a>返回流量</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p13551332727"><a name="zh-cn_topic_0015479905_p13551332727"></a><a name="zh-cn_topic_0015479905_p13551332727"></a>该指标用于统计测量api接口返回流量。</p>
<p id="zh-cn_topic_0015479905_p159737141202"><a name="zh-cn_topic_0015479905_p159737141202"></a><a name="zh-cn_topic_0015479905_p159737141202"></a>单位：字节</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p189465496111"><a name="zh-cn_topic_0015479905_p189465496111"></a><a name="zh-cn_topic_0015479905_p189465496111"></a>≥ 0 byte</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p55713215214"><a name="zh-cn_topic_0015479905_p55713215214"></a><a name="zh-cn_topic_0015479905_p55713215214"></a>api接口</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p11701115813367"><a name="zh-cn_topic_0015479905_p11701115813367"></a><a name="zh-cn_topic_0015479905_p11701115813367"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row11801632823"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p78451256936"><a name="zh-cn_topic_0015479905_p78451256936"></a><a name="zh-cn_topic_0015479905_p78451256936"></a>请求流量</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p146116323213"><a name="zh-cn_topic_0015479905_p146116323213"></a><a name="zh-cn_topic_0015479905_p146116323213"></a>该指标用于统计测量api接口请求流量。</p>
<p id="zh-cn_topic_0015479905_p19537175312594"><a name="zh-cn_topic_0015479905_p19537175312594"></a><a name="zh-cn_topic_0015479905_p19537175312594"></a>单位：字节</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p2948154917114"><a name="zh-cn_topic_0015479905_p2948154917114"></a><a name="zh-cn_topic_0015479905_p2948154917114"></a>≥ 0 byte</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p36312327212"><a name="zh-cn_topic_0015479905_p36312327212"></a><a name="zh-cn_topic_0015479905_p36312327212"></a>api接口</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p2074275893614"><a name="zh-cn_topic_0015479905_p2074275893614"></a><a name="zh-cn_topic_0015479905_p2074275893614"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0015479905_row117717327218"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0015479905_p1184595615310"><a name="zh-cn_topic_0015479905_p1184595615310"></a><a name="zh-cn_topic_0015479905_p1184595615310"></a>总的错误次数</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0015479905_p96623219215"><a name="zh-cn_topic_0015479905_p96623219215"></a><a name="zh-cn_topic_0015479905_p96623219215"></a>该指标用于统计测量api接口总的错误次数。</p>
<p id="zh-cn_topic_0015479905_p617124255913"><a name="zh-cn_topic_0015479905_p617124255913"></a><a name="zh-cn_topic_0015479905_p617124255913"></a>单位：次/分钟</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0015479905_p1122145541119"><a name="zh-cn_topic_0015479905_p1122145541119"></a><a name="zh-cn_topic_0015479905_p1122145541119"></a>≥ 0 times/min</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0015479905_p1968532728"><a name="zh-cn_topic_0015479905_p1968532728"></a><a name="zh-cn_topic_0015479905_p1968532728"></a>api接口</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0015479905_p3791758113619"><a name="zh-cn_topic_0015479905_p3791758113619"></a><a name="zh-cn_topic_0015479905_p3791758113619"></a>1分钟</p>
</td>
</tr>
</tbody>
</table>

