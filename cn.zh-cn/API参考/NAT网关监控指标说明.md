# NAT网关监控指标说明<a name="ZH-CN_TOPIC_0102475743"></a>

## 功能说明<a name="section59820001153251"></a>

本节定义了NAT网关上报云监控的监控指标的命名空间，监控指标列表和维度定义，用户可以通过云监控提供的API接口来检索NAT网关产生的监控指标。

## 命名空间<a name="section172651386227"></a>

SYS.NAT

## 监控指标<a name="section18266133811225"></a>

<a name="table102675383222"></a>
<table><thead align="left"><tr id="row726893842214"><th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.1.6.1.1"><p id="p20269183892219"><a name="p20269183892219"></a><a name="p20269183892219"></a>指标</p>
</th>
<th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.6.1.2"><p id="p16270153816220"><a name="p16270153816220"></a><a name="p16270153816220"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="36.36363636363637%" id="mcps1.1.6.1.3"><p id="p527115383221"><a name="p527115383221"></a><a name="p527115383221"></a>含义</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.1.6.1.4"><p id="p202711238192210"><a name="p202711238192210"></a><a name="p202711238192210"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="21.21212121212121%" id="mcps1.1.6.1.5"><p id="p52723385226"><a name="p52723385226"></a><a name="p52723385226"></a>测量对象</p>
</th>
</tr>
</thead>
<tbody><tr id="row2272193812219"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.6.1.1 "><p id="p149641356171117"><a name="p149641356171117"></a><a name="p149641356171117"></a>snat_connection</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.6.1.2 "><p id="p59647568111"><a name="p59647568111"></a><a name="p59647568111"></a>SNAT连接数</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363637%" headers="mcps1.1.6.1.3 "><p id="p14964956111116"><a name="p14964956111116"></a><a name="p14964956111116"></a>该指标用于统计测量对象的SNAT连接数。</p>
<p id="p7369230172013"><a name="p7369230172013"></a><a name="p7369230172013"></a>单位：count</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.1.6.1.4 "><p id="p896412563116"><a name="p896412563116"></a><a name="p896412563116"></a>≥ 0 count</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.6.1.5 "><p id="p1964356101112"><a name="p1964356101112"></a><a name="p1964356101112"></a>NAT网关主节点</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="section102905383226"></a>

<a name="table13291038182217"></a>
<table><thead align="left"><tr id="row13292153862219"><th class="cellrowborder" valign="top" width="40.400000000000006%" id="mcps1.1.3.1.1"><p id="p17292638192211"><a name="p17292638192211"></a><a name="p17292638192211"></a>Key</p>
</th>
<th class="cellrowborder" valign="top" width="59.599999999999994%" id="mcps1.1.3.1.2"><p id="p92938385226"><a name="p92938385226"></a><a name="p92938385226"></a>Value</p>
</th>
</tr>
</thead>
<tbody><tr id="row1429373812228"><td class="cellrowborder" valign="top" width="40.400000000000006%" headers="mcps1.1.3.1.1 "><p id="p11777171991217"><a name="p11777171991217"></a><a name="p11777171991217"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="59.599999999999994%" headers="mcps1.1.3.1.2 "><p id="p11777101931217"><a name="p11777101931217"></a><a name="p11777101931217"></a>NAT网关实例标识</p>
</td>
</tr>
</tbody>
</table>

