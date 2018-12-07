# Cron表达式取值说明<a name="ZH-CN_TOPIC_0139089704"></a>

在ECS资源中，您可以通过Cron表达式设置一些基于时间的日程安排程序。您可以在云助手中，通过设置具有Cron表达式的参数完成一些周期性任务、固定的日常任务或者在某个准确的时间完成单次任务。

## Cron表达式取值说明<a name="section1957201335418"></a>

Cron 表达式是一个具有时间含义的字符串（String），字符串以4个空格隔开，分为5个字段，格式为X X X X X。其中X表示一个字段的占位符，单个字段有多个取值时，使用半角逗号,隔开取值。每个字段可以是确定的取值，也可以是具有逻辑意义的特殊字符。[表1](#table88353370547)为Cron表达式中5个字符能够取的值以及支持的特殊字符，特殊字符说明请参见[表2](#table698212121020)，Cron表达式取值示例请参见[表3](#table109651335191415)。

**表 1**  Cron表达式取值说明

<a name="table88353370547"></a>
<table><thead align="left"><tr id="row28361237175416"><th class="cellrowborder" valign="top" width="14.270000000000001%" id="mcps1.2.5.1.1"><p id="p1583612378547"><a name="p1583612378547"></a><a name="p1583612378547"></a>字段</p>
</th>
<th class="cellrowborder" valign="top" width="14.270000000000001%" id="mcps1.2.5.1.2"><p id="p13836837195420"><a name="p13836837195420"></a><a name="p13836837195420"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="46.34%" id="mcps1.2.5.1.3"><p id="p188361137195413"><a name="p188361137195413"></a><a name="p188361137195413"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="25.120000000000005%" id="mcps1.2.5.1.4"><p id="p8836193716541"><a name="p8836193716541"></a><a name="p8836193716541"></a>特殊字符</p>
</th>
</tr>
</thead>
<tbody><tr id="row7836153718542"><td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.1 "><p id="p4114183010557"><a name="p4114183010557"></a><a name="p4114183010557"></a>分</p>
</td>
<td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.2 "><p id="p51141630155520"><a name="p51141630155520"></a><a name="p51141630155520"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="46.34%" headers="mcps1.2.5.1.3 "><p id="p5114133011554"><a name="p5114133011554"></a><a name="p5114133011554"></a>0-59</p>
</td>
<td class="cellrowborder" valign="top" width="25.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p911443075515"><a name="p911443075515"></a><a name="p911443075515"></a>* , - /</p>
</td>
</tr>
<tr id="row583653785412"><td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.1 "><p id="p1511443013558"><a name="p1511443013558"></a><a name="p1511443013558"></a>小时</p>
</td>
<td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.2 "><p id="p1811413016554"><a name="p1811413016554"></a><a name="p1811413016554"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="46.34%" headers="mcps1.2.5.1.3 "><p id="p1511411308554"><a name="p1511411308554"></a><a name="p1511411308554"></a>0-23</p>
</td>
<td class="cellrowborder" valign="top" width="25.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p511473018558"><a name="p511473018558"></a><a name="p511473018558"></a>* , - /</p>
</td>
</tr>
<tr id="row118361337125418"><td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.1 "><p id="p5114153015551"><a name="p5114153015551"></a><a name="p5114153015551"></a>日期</p>
</td>
<td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.2 "><p id="p5114530135514"><a name="p5114530135514"></a><a name="p5114530135514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="46.34%" headers="mcps1.2.5.1.3 "><p id="p811463015517"><a name="p811463015517"></a><a name="p811463015517"></a>1-31</p>
</td>
<td class="cellrowborder" valign="top" width="25.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p61146300555"><a name="p61146300555"></a><a name="p61146300555"></a>* , - / ?</p>
</td>
</tr>
<tr id="row883615372546"><td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.1 "><p id="p1211483016553"><a name="p1211483016553"></a><a name="p1211483016553"></a>月份</p>
</td>
<td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.2 "><p id="p16114130185520"><a name="p16114130185520"></a><a name="p16114130185520"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="46.34%" headers="mcps1.2.5.1.3 "><p id="p6114930165517"><a name="p6114930165517"></a><a name="p6114930165517"></a>1-12或JAN-DEC</p>
</td>
<td class="cellrowborder" valign="top" width="25.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p6114830175519"><a name="p6114830175519"></a><a name="p6114830175519"></a>* , - /</p>
</td>
</tr>
<tr id="row148385375548"><td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.1 "><p id="p161151030185516"><a name="p161151030185516"></a><a name="p161151030185516"></a>星期</p>
</td>
<td class="cellrowborder" valign="top" width="14.270000000000001%" headers="mcps1.2.5.1.2 "><p id="p3115193010554"><a name="p3115193010554"></a><a name="p3115193010554"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="46.34%" headers="mcps1.2.5.1.3 "><p id="p78621449133812"><a name="p78621449133812"></a><a name="p78621449133812"></a>1-7或 SUN-SAT</p>
<p id="p211519305552"><a name="p211519305552"></a><a name="p211519305552"></a>若使用1-7，1代表星期天，2 代表星期一。</p>
</td>
<td class="cellrowborder" valign="top" width="25.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p14115173014550"><a name="p14115173014550"></a><a name="p14115173014550"></a>* , - / ?</p>
</td>
</tr>
</tbody>
</table>

**表 2**  特殊字符说明

<a name="table698212121020"></a>
<table><thead align="left"><tr id="row598510181017"><th class="cellrowborder" valign="top" width="19.23%" id="mcps1.2.3.1.1"><p id="p13985116107"><a name="p13985116107"></a><a name="p13985116107"></a>特殊字符</p>
</th>
<th class="cellrowborder" valign="top" width="80.77%" id="mcps1.2.3.1.2"><p id="p15985151161018"><a name="p15985151161018"></a><a name="p15985151161018"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row20985121151017"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p29851518104"><a name="p29851518104"></a><a name="p29851518104"></a>*</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p7609151531118"><a name="p7609151531118"></a><a name="p7609151531118"></a>表示所有可能的值。</p>
<p id="p3610121541117"><a name="p3610121541117"></a><a name="p3610121541117"></a>例如在字段 “月” 中“*”表示每个月。</p>
</td>
</tr>
<tr id="row18985817106"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p1598551161018"><a name="p1598551161018"></a><a name="p1598551161018"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p12285193011114"><a name="p12285193011114"></a><a name="p12285193011114"></a>表示指定范围。</p>
<p id="p16287143001117"><a name="p16287143001117"></a><a name="p16287143001117"></a>例如在字段“分”里，"5-20"表示5分到20分钟之间每隔一分钟执行一次。</p>
</td>
</tr>
<tr id="row89857111011"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p139854121019"><a name="p139854121019"></a><a name="p139854121019"></a>,</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p2394163661117"><a name="p2394163661117"></a><a name="p2394163661117"></a>表示列出枚举值。</p>
<p id="p6394153615112"><a name="p6394153615112"></a><a name="p6394153615112"></a>例如在字段“分”里，"5,20"表示第5分钟和第20分钟执行。</p>
</td>
</tr>
<tr id="row798517171016"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p199856118108"><a name="p199856118108"></a><a name="p199856118108"></a>/</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p16458164412119"><a name="p16458164412119"></a><a name="p16458164412119"></a>表示指定数值的增量。</p>
<p id="p1245811442115"><a name="p1245811442115"></a><a name="p1245811442115"></a>例如在字段“分”里，"5/20"表示从第5分钟起，每隔20分钟执行一次。</p>
</td>
</tr>
<tr id="row398519115101"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p15985916102"><a name="p15985916102"></a><a name="p15985916102"></a>?</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p09857151010"><a name="p09857151010"></a><a name="p09857151010"></a>表示不指定具体值，仅在字段“日期”和“星期”中使用。当字段“日期” 或者 “星期” 其中之一被指定了值以后，为了避免冲突，需要将另一个字段的值设为？。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  Corn表达式取值示例

<a name="table109651335191415"></a>
<table><thead align="left"><tr id="row199678357146"><th class="cellrowborder" valign="top" width="19.23%" id="mcps1.2.3.1.1"><p id="p189691035101416"><a name="p189691035101416"></a><a name="p189691035101416"></a>示例</p>
</th>
<th class="cellrowborder" valign="top" width="80.77%" id="mcps1.2.3.1.2"><p id="p296911354144"><a name="p296911354144"></a><a name="p296911354144"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19970183519148"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p297263519146"><a name="p297263519146"></a><a name="p297263519146"></a>10 12 ? * *</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p1597393511415"><a name="p1597393511415"></a><a name="p1597393511415"></a>每天上午12:10执行命令。</p>
</td>
</tr>
<tr id="row5973173516145"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p179752355146"><a name="p179752355146"></a><a name="p179752355146"></a>10 12 * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p18656153071718"><a name="p18656153071718"></a><a name="p18656153071718"></a>每天上午10:15执行命令。</p>
</td>
</tr>
<tr id="row29887354149"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p12990173551413"><a name="p12990173551413"></a><a name="p12990173551413"></a>0 11,12,13 * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p139901735201416"><a name="p139901735201416"></a><a name="p139901735201416"></a>每天11:00、12:00 、13:00执行命令。</p>
</td>
</tr>
<tr id="row1299112351141"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p1599163561411"><a name="p1599163561411"></a><a name="p1599163561411"></a>0/15 10-18 * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p149931435101417"><a name="p149931435101417"></a><a name="p149931435101417"></a>每天10:00到18:00时间段内每隔15分钟执行命令。</p>
</td>
</tr>
<tr id="row129934354143"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p1599518358144"><a name="p1599518358144"></a><a name="p1599518358144"></a>* 16 * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p1899573541414"><a name="p1899573541414"></a><a name="p1899573541414"></a>每天16:00到16:59时间段内每隔1分钟执行命令。</p>
</td>
</tr>
<tr id="row6995113519147"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p1099719353146"><a name="p1099719353146"></a><a name="p1099719353146"></a>0/5 10,14 * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p159981354149"><a name="p159981354149"></a><a name="p159981354149"></a>每天10:00到10:55 、14:00到14:55时间段内每隔5分钟执行命令。</p>
</td>
</tr>
<tr id="row52113610145"><td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.3.1.1 "><p id="p172836141417"><a name="p172836141417"></a><a name="p172836141417"></a>0 10 12 ? * MON-FRI</p>
</td>
<td class="cellrowborder" valign="top" width="80.77%" headers="mcps1.2.3.1.2 "><p id="p1390338163015"><a name="p1390338163015"></a><a name="p1390338163015"></a>周一到周五每天12:10执行命令。</p>
</td>
</tr>
</tbody>
</table>

