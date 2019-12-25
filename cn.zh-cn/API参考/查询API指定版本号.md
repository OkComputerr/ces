# 查询API指定版本号<a name="ZH-CN_TOPIC_0171212610"></a>

## 功能介绍<a name="section66578044"></a>

查询云监控API指定版本号。

## URI<a name="section62331491"></a>

GET /\{api\_version\}

-   参数说明

    **表 1**  参数说明

    <a name="table23820074175412"></a>
    <table><thead align="left"><tr id="row17704405175412"><th class="cellrowborder" valign="top" width="19.99%" id="mcps1.2.4.1.1"><p id="p24770673175412"><a name="p24770673175412"></a><a name="p24770673175412"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.93%" id="mcps1.2.4.1.2"><p id="p60267522175412"><a name="p60267522175412"></a><a name="p60267522175412"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="59.08%" id="mcps1.2.4.1.3"><p id="p49831152175412"><a name="p49831152175412"></a><a name="p49831152175412"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row9791522175412"><td class="cellrowborder" valign="top" width="19.99%" headers="mcps1.2.4.1.1 "><p id="p54915841175412"><a name="p54915841175412"></a><a name="p54915841175412"></a>api_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.93%" headers="mcps1.2.4.1.2 "><p id="p18998132175412"><a name="p18998132175412"></a><a name="p18998132175412"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="59.08%" headers="mcps1.2.4.1.3 "><p id="p62453732175412"><a name="p62453732175412"></a><a name="p62453732175412"></a>API版本号。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   样例

    ```
    GET https://{Cloud Eye的endpoint}/V1.0
    ```


## 请求消息<a name="section24112512"></a>

无

## 响应消息<a name="section15686020"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table26246518152631"></a>
    <table><thead align="left"><tr id="row29602547152631"><th class="cellrowborder" valign="top" width="18.72%" id="mcps1.2.4.1.1"><p id="p1143665616354"><a name="p1143665616354"></a><a name="p1143665616354"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.73%" id="mcps1.2.4.1.2"><p id="p11440156143517"><a name="p11440156143517"></a><a name="p11440156143517"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="63.55%" id="mcps1.2.4.1.3"><p id="p244212561357"><a name="p244212561357"></a><a name="p244212561357"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row56174697152631"><td class="cellrowborder" valign="top" width="18.72%" headers="mcps1.2.4.1.1 "><p id="p4445556153516"><a name="p4445556153516"></a><a name="p4445556153516"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.73%" headers="mcps1.2.4.1.2 "><p id="p444855610353"><a name="p444855610353"></a><a name="p444855610353"></a>Objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.55%" headers="mcps1.2.4.1.3 "><p id="p344911569354"><a name="p344911569354"></a><a name="p344911569354"></a>描述version 相关对象。</p>
    <p id="p76411522123610"><a name="p76411522123610"></a><a name="p76411522123610"></a>详细参数说明请参见<a href="#table697164712507">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  versions字段数据结构说明

    <a name="table697164712507"></a>
    <table><thead align="left"><tr id="row1898124785019"><th class="cellrowborder" valign="top" width="18.72%" id="mcps1.2.4.1.1"><p id="p4981247195018"><a name="p4981247195018"></a><a name="p4981247195018"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.73%" id="mcps1.2.4.1.2"><p id="p79844713504"><a name="p79844713504"></a><a name="p79844713504"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="63.55%" id="mcps1.2.4.1.3"><p id="p698194713501"><a name="p698194713501"></a><a name="p698194713501"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row89854714509"><td class="cellrowborder" valign="top" width="18.72%" headers="mcps1.2.4.1.1 "><p id="p139834735010"><a name="p139834735010"></a><a name="p139834735010"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.73%" headers="mcps1.2.4.1.2 "><p id="p298114755020"><a name="p298114755020"></a><a name="p298114755020"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.55%" headers="mcps1.2.4.1.3 "><p id="p179964715014"><a name="p179964715014"></a><a name="p179964715014"></a>版本ID（版本号），如v1。</p>
    </td>
    </tr>
    <tr id="row299164795019"><td class="cellrowborder" valign="top" width="18.72%" headers="mcps1.2.4.1.1 "><p id="p199919474509"><a name="p199919474509"></a><a name="p199919474509"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.73%" headers="mcps1.2.4.1.2 "><p id="p8991047175014"><a name="p8991047175014"></a><a name="p8991047175014"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.55%" headers="mcps1.2.4.1.3 "><p id="p59964795019"><a name="p59964795019"></a><a name="p59964795019"></a>API的URL地址。</p>
    <p id="p181431404541"><a name="p181431404541"></a><a name="p181431404541"></a>详细参数说明请参见<a href="#table826514508503">表4</a>。</p>
    </td>
    </tr>
    <tr id="row79914725015"><td class="cellrowborder" valign="top" width="18.72%" headers="mcps1.2.4.1.1 "><p id="p199974711501"><a name="p199974711501"></a><a name="p199974711501"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.73%" headers="mcps1.2.4.1.2 "><p id="p12992477506"><a name="p12992477506"></a><a name="p12992477506"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.55%" headers="mcps1.2.4.1.3 "><p id="p1613574610538"><a name="p1613574610538"></a><a name="p1613574610538"></a>若该版本API支持微版本，该参数表示支持的最大微版本号，如果不支持微版本，则为空。</p>
    </td>
    </tr>
    <tr id="row1910011478501"><td class="cellrowborder" valign="top" width="18.72%" headers="mcps1.2.4.1.1 "><p id="p4100134718509"><a name="p4100134718509"></a><a name="p4100134718509"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.73%" headers="mcps1.2.4.1.2 "><p id="p110019470505"><a name="p110019470505"></a><a name="p110019470505"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.55%" headers="mcps1.2.4.1.3 "><p id="p1210024725017"><a name="p1210024725017"></a><a name="p1210024725017"></a>版本状态，为如下3种：</p>
    <p id="p1010024712509"><a name="p1010024712509"></a><a name="p1010024712509"></a>CURRENT：表示该版本为主推版本。</p>
    <p id="p210054735017"><a name="p210054735017"></a><a name="p210054735017"></a>SUPPORTED：表示为老版本，但是现在还继续支持。</p>
    <p id="p1100047125014"><a name="p1100047125014"></a><a name="p1100047125014"></a>DEPRECATED：表示为废弃版本，存在后续删除的可能。</p>
    </td>
    </tr>
    <tr id="row1310017478505"><td class="cellrowborder" valign="top" width="18.72%" headers="mcps1.2.4.1.1 "><p id="p3100154715016"><a name="p3100154715016"></a><a name="p3100154715016"></a>updated</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.73%" headers="mcps1.2.4.1.2 "><p id="p141001847135012"><a name="p141001847135012"></a><a name="p141001847135012"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.55%" headers="mcps1.2.4.1.3 "><p id="p9100164765020"><a name="p9100164765020"></a><a name="p9100164765020"></a>版本发布时间，采用UTC时间表示。如v1发布的时间2014-06-28T12:20:21Z。</p>
    </td>
    </tr>
    <tr id="row5100144717502"><td class="cellrowborder" valign="top" width="18.72%" headers="mcps1.2.4.1.1 "><p id="p1310010474502"><a name="p1310010474502"></a><a name="p1310010474502"></a>min_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.73%" headers="mcps1.2.4.1.2 "><p id="p7100134735019"><a name="p7100134735019"></a><a name="p7100134735019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.55%" headers="mcps1.2.4.1.3 "><p id="p7556103913538"><a name="p7556103913538"></a><a name="p7556103913538"></a>若该版本API 支持微版本，该参数表示支持的最小微版本号， 如果不支持微版本，则为空。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  links字段数据结构说明

    <a name="table826514508503"></a>
    <table><thead align="left"><tr id="row15266125018507"><th class="cellrowborder" valign="top" width="18.72%" id="mcps1.2.4.1.1"><p id="p726618502508"><a name="p726618502508"></a><a name="p726618502508"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.73%" id="mcps1.2.4.1.2"><p id="p11266135011504"><a name="p11266135011504"></a><a name="p11266135011504"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="63.55%" id="mcps1.2.4.1.3"><p id="p726625019507"><a name="p726625019507"></a><a name="p726625019507"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row16267105014508"><td class="cellrowborder" valign="top" width="18.72%" headers="mcps1.2.4.1.1 "><p id="p726735018501"><a name="p726735018501"></a><a name="p726735018501"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.73%" headers="mcps1.2.4.1.2 "><p id="p1526745015503"><a name="p1526745015503"></a><a name="p1526745015503"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.55%" headers="mcps1.2.4.1.3 "><p id="p1726735085010"><a name="p1726735085010"></a><a name="p1726735085010"></a>当前API版本的引用地址。</p>
    </td>
    </tr>
    <tr id="row1326725018501"><td class="cellrowborder" valign="top" width="18.72%" headers="mcps1.2.4.1.1 "><p id="p72674509503"><a name="p72674509503"></a><a name="p72674509503"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.73%" headers="mcps1.2.4.1.2 "><p id="p132670509503"><a name="p132670509503"></a><a name="p132670509503"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.55%" headers="mcps1.2.4.1.3 "><p id="p15267750125020"><a name="p15267750125020"></a><a name="p15267750125020"></a>当前API版本和被引用地址的关系。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    { 
      "version": { 
          "id": "V1.0", 
          "links": [ 
            { 
              "href": "https://x.x.x.x/V1.0/", 
              "rel": "self" 
            } 
          ], 
          "min_version": "", 
          "status": "CURRENT", 
          "updated": "2018-09-30T00:00:00Z", 
          "version": "" 
        } 
    }
    ```


## 返回值<a name="section6956456"></a>

-   正常

    200

-   异常

    <a name="table46793998"></a>
    <table><thead align="left"><tr id="row65573909"><th class="cellrowborder" valign="top" width="34.44%" id="mcps1.1.3.1.1"><p id="p9886408"><a name="p9886408"></a><a name="p9886408"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="65.56%" id="mcps1.1.3.1.2"><p id="p62601592"><a name="p62601592"></a><a name="p62601592"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row37564172"><td class="cellrowborder" valign="top" width="34.44%" headers="mcps1.1.3.1.1 "><p id="p22799085"><a name="p22799085"></a><a name="p22799085"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.56%" headers="mcps1.1.3.1.2 "><p id="p44643603"><a name="p44643603"></a><a name="p44643603"></a>请求错误。</p>
    </td>
    </tr>
    <tr id="row66248115"><td class="cellrowborder" valign="top" width="34.44%" headers="mcps1.1.3.1.1 "><p id="p64497130"><a name="p64497130"></a><a name="p64497130"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.56%" headers="mcps1.1.3.1.2 "><p id="p42202994"><a name="p42202994"></a><a name="p42202994"></a>未提供认证信息，或认证信息错误。</p>
    </td>
    </tr>
    <tr id="row44282627"><td class="cellrowborder" valign="top" width="34.44%" headers="mcps1.1.3.1.1 "><p id="p30123063"><a name="p30123063"></a><a name="p30123063"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.56%" headers="mcps1.1.3.1.2 "><p id="p15114764"><a name="p15114764"></a><a name="p15114764"></a>请求页面被禁止访问。</p>
    </td>
    </tr>
    <tr id="row1815156"><td class="cellrowborder" valign="top" width="34.44%" headers="mcps1.1.3.1.1 "><p id="p12809933"><a name="p12809933"></a><a name="p12809933"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.56%" headers="mcps1.1.3.1.2 "><p id="p10309404"><a name="p10309404"></a><a name="p10309404"></a>请求超出了服务器的等待时间。</p>
    </td>
    </tr>
    <tr id="row25675773"><td class="cellrowborder" valign="top" width="34.44%" headers="mcps1.1.3.1.1 "><p id="p66471715"><a name="p66471715"></a><a name="p66471715"></a>429 Too Many Requests</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.56%" headers="mcps1.1.3.1.2 "><p id="p5281111"><a name="p5281111"></a><a name="p5281111"></a>当前请求过多。</p>
    </td>
    </tr>
    <tr id="row47530006"><td class="cellrowborder" valign="top" width="34.44%" headers="mcps1.1.3.1.1 "><p id="p24725298"><a name="p24725298"></a><a name="p24725298"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.56%" headers="mcps1.1.3.1.2 "><p id="p39567352"><a name="p39567352"></a><a name="p39567352"></a>请求未完成，服务异常。</p>
    </td>
    </tr>
    <tr id="row20561848"><td class="cellrowborder" valign="top" width="34.44%" headers="mcps1.1.3.1.1 "><p id="p54897010"><a name="p54897010"></a><a name="p54897010"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.56%" headers="mcps1.1.3.1.2 "><p id="p1451523117958"><a name="p1451523117958"></a><a name="p1451523117958"></a>系统暂时不可用，请求受限。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 错误码<a name="section137621219143417"></a>

请参考[返回错误码说明](返回错误码说明.md)。

