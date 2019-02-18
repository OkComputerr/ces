# 查询API指定版本号<a name="ZH-CN_TOPIC_0133184491"></a>

## 功能介绍<a name="section66578044"></a>

查询云监控API指定版本号。

## URI<a name="section62331491"></a>

GET/\{api\_version\}

-   参数说明

    **表 1**  参数说明

    <a name="table23820074175412"></a>
    <table><thead align="left"><tr id="row17704405175412"><th class="cellrowborder" valign="top" width="25.281396231187557%" id="mcps1.2.3.1.1"><p id="p24770673175412"><a name="p24770673175412"></a><a name="p24770673175412"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="74.71860376881246%" id="mcps1.2.3.1.2"><p id="p49831152175412"><a name="p49831152175412"></a><a name="p49831152175412"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row9791522175412"><td class="cellrowborder" valign="top" width="25.281396231187557%" headers="mcps1.2.3.1.1 "><p id="p54915841175412"><a name="p54915841175412"></a><a name="p54915841175412"></a>api_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.71860376881246%" headers="mcps1.2.3.1.2 "><p id="p62453732175412"><a name="p62453732175412"></a><a name="p62453732175412"></a>API版本号。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   样例

    ```
    /V1.0
    ```


## 请求消息<a name="section24112512"></a>

无

## 响应消息<a name="section15686020"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table26246518152631"></a>
    <table><thead align="left"><tr id="row29602547152631"><th class="cellrowborder" valign="top" width="27.889185116494726%" id="mcps1.2.4.1.1"><p id="p1143665616354"><a name="p1143665616354"></a><a name="p1143665616354"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.95212704300452%" id="mcps1.2.4.1.2"><p id="p11440156143517"><a name="p11440156143517"></a><a name="p11440156143517"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.158687840500754%" id="mcps1.2.4.1.3"><p id="p244212561357"><a name="p244212561357"></a><a name="p244212561357"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row56174697152631"><td class="cellrowborder" valign="top" width="27.889185116494726%" headers="mcps1.2.4.1.1 "><p id="p4445556153516"><a name="p4445556153516"></a><a name="p4445556153516"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95212704300452%" headers="mcps1.2.4.1.2 "><p id="p444855610353"><a name="p444855610353"></a><a name="p444855610353"></a>字典数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.158687840500754%" headers="mcps1.2.4.1.3 "><p id="p344911569354"><a name="p344911569354"></a><a name="p344911569354"></a>描述version 相关对象。</p>
    </td>
    </tr>
    <tr id="row4615503152631"><td class="cellrowborder" valign="top" width="27.889185116494726%" headers="mcps1.2.4.1.1 "><p id="p8452756123518"><a name="p8452756123518"></a><a name="p8452756123518"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95212704300452%" headers="mcps1.2.4.1.2 "><p id="p1445545663515"><a name="p1445545663515"></a><a name="p1445545663515"></a>字符串</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.158687840500754%" headers="mcps1.2.4.1.3 "><p id="p045585620357"><a name="p045585620357"></a><a name="p045585620357"></a>版本ID（版本号），如v1。</p>
    </td>
    </tr>
    <tr id="row9239644152631"><td class="cellrowborder" valign="top" width="27.889185116494726%" headers="mcps1.2.4.1.1 "><p id="p9460175653518"><a name="p9460175653518"></a><a name="p9460175653518"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95212704300452%" headers="mcps1.2.4.1.2 "><p id="p346325618353"><a name="p346325618353"></a><a name="p346325618353"></a>数组</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.158687840500754%" headers="mcps1.2.4.1.3 "><p id="p746525619351"><a name="p746525619351"></a><a name="p746525619351"></a>API的URL地址。</p>
    </td>
    </tr>
    <tr id="row419672501413"><td class="cellrowborder" valign="top" width="27.889185116494726%" headers="mcps1.2.4.1.1 "><p id="p16283354130"><a name="p16283354130"></a><a name="p16283354130"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95212704300452%" headers="mcps1.2.4.1.2 "><p id="p13242332181317"><a name="p13242332181317"></a><a name="p13242332181317"></a>字符串</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.158687840500754%" headers="mcps1.2.4.1.3 "><p id="p2269104581219"><a name="p2269104581219"></a><a name="p2269104581219"></a>当前API版本的引用地址。</p>
    </td>
    </tr>
    <tr id="row154810286148"><td class="cellrowborder" valign="top" width="27.889185116494726%" headers="mcps1.2.4.1.1 "><p id="p2139956101218"><a name="p2139956101218"></a><a name="p2139956101218"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95212704300452%" headers="mcps1.2.4.1.2 "><p id="p824653211138"><a name="p824653211138"></a><a name="p824653211138"></a>字符串</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.158687840500754%" headers="mcps1.2.4.1.3 "><p id="p513917563125"><a name="p513917563125"></a><a name="p513917563125"></a>当前API版本和被引用地址的关系。</p>
    </td>
    </tr>
    <tr id="row12929787152631"><td class="cellrowborder" valign="top" width="27.889185116494726%" headers="mcps1.2.4.1.1 "><p id="p13468556113518"><a name="p13468556113518"></a><a name="p13468556113518"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95212704300452%" headers="mcps1.2.4.1.2 "><p id="p18472756113513"><a name="p18472756113513"></a><a name="p18472756113513"></a>字符串</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.158687840500754%" headers="mcps1.2.4.1.3 "><p id="p11474856173511"><a name="p11474856173511"></a><a name="p11474856173511"></a>若该版本API支持微版本，则填支持的最大微版本号，如果不支持微版本，则填空</p>
    </td>
    </tr>
    <tr id="row39341340152631"><td class="cellrowborder" valign="top" width="27.889185116494726%" headers="mcps1.2.4.1.1 "><p id="p647516561358"><a name="p647516561358"></a><a name="p647516561358"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95212704300452%" headers="mcps1.2.4.1.2 "><p id="p164801756103517"><a name="p164801756103517"></a><a name="p164801756103517"></a>字符串</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.158687840500754%" headers="mcps1.2.4.1.3 "><p id="p104811756113517"><a name="p104811756113517"></a><a name="p104811756113517"></a>版本状态，为如下3种：</p>
    <p id="p10482145613510"><a name="p10482145613510"></a><a name="p10482145613510"></a>CURRENT：表示该版本为主推版本。</p>
    <p id="p9483556103513"><a name="p9483556103513"></a><a name="p9483556103513"></a>SUPPORTED：表示为老版本，但是现在还继续支持。</p>
    <p id="p18484105612355"><a name="p18484105612355"></a><a name="p18484105612355"></a>DEPRECATED：表示为废弃版本，存在后续删除的可能。</p>
    </td>
    </tr>
    <tr id="row398200152631"><td class="cellrowborder" valign="top" width="27.889185116494726%" headers="mcps1.2.4.1.1 "><p id="p7486145617358"><a name="p7486145617358"></a><a name="p7486145617358"></a>updated</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95212704300452%" headers="mcps1.2.4.1.2 "><p id="p34901556173518"><a name="p34901556173518"></a><a name="p34901556173518"></a>字符串</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.158687840500754%" headers="mcps1.2.4.1.3 "><p id="p24932056163517"><a name="p24932056163517"></a><a name="p24932056163517"></a>版本发布时间，要求用UTC时间表示。如v1发布的时间2014-06-28T12:20:21Z。</p>
    </td>
    </tr>
    <tr id="row61549520152631"><td class="cellrowborder" valign="top" width="27.889185116494726%" headers="mcps1.2.4.1.1 "><p id="p2495115693510"><a name="p2495115693510"></a><a name="p2495115693510"></a>min_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95212704300452%" headers="mcps1.2.4.1.2 "><p id="p134991256203512"><a name="p134991256203512"></a><a name="p134991256203512"></a>字符串</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.158687840500754%" headers="mcps1.2.4.1.3 "><p id="p205014565351"><a name="p205014565351"></a><a name="p205014565351"></a>若该版本API 支持微版本，则填支持的最小微版本号， 如果不支持微版本，则填空。</p>
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
    <table><thead align="left"><tr id="row65573909"><th class="cellrowborder" valign="top" width="61.839999999999996%" id="mcps1.1.3.1.1"><p id="p9886408"><a name="p9886408"></a><a name="p9886408"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.16%" id="mcps1.1.3.1.2"><p id="p62601592"><a name="p62601592"></a><a name="p62601592"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row37564172"><td class="cellrowborder" valign="top" width="61.839999999999996%" headers="mcps1.1.3.1.1 "><p id="p22799085"><a name="p22799085"></a><a name="p22799085"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.16%" headers="mcps1.1.3.1.2 "><p id="p44643603"><a name="p44643603"></a><a name="p44643603"></a>请求错误。</p>
    </td>
    </tr>
    <tr id="row66248115"><td class="cellrowborder" valign="top" width="61.839999999999996%" headers="mcps1.1.3.1.1 "><p id="p64497130"><a name="p64497130"></a><a name="p64497130"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.16%" headers="mcps1.1.3.1.2 "><p id="p42202994"><a name="p42202994"></a><a name="p42202994"></a>未提供认证信息，或认证信息错。</p>
    </td>
    </tr>
    <tr id="row44282627"><td class="cellrowborder" valign="top" width="61.839999999999996%" headers="mcps1.1.3.1.1 "><p id="p30123063"><a name="p30123063"></a><a name="p30123063"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.16%" headers="mcps1.1.3.1.2 "><p id="p15114764"><a name="p15114764"></a><a name="p15114764"></a>请求页面被禁止访问。</p>
    </td>
    </tr>
    <tr id="row1815156"><td class="cellrowborder" valign="top" width="61.839999999999996%" headers="mcps1.1.3.1.1 "><p id="p12809933"><a name="p12809933"></a><a name="p12809933"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.16%" headers="mcps1.1.3.1.2 "><p id="p10309404"><a name="p10309404"></a><a name="p10309404"></a>请求超出了服务器的等待时间。</p>
    </td>
    </tr>
    <tr id="row25675773"><td class="cellrowborder" valign="top" width="61.839999999999996%" headers="mcps1.1.3.1.1 "><p id="p66471715"><a name="p66471715"></a><a name="p66471715"></a>429 Too Many Requests</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.16%" headers="mcps1.1.3.1.2 "><p id="p5281111"><a name="p5281111"></a><a name="p5281111"></a>当前请求过多。</p>
    </td>
    </tr>
    <tr id="row47530006"><td class="cellrowborder" valign="top" width="61.839999999999996%" headers="mcps1.1.3.1.1 "><p id="p24725298"><a name="p24725298"></a><a name="p24725298"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.16%" headers="mcps1.1.3.1.2 "><p id="p39567352"><a name="p39567352"></a><a name="p39567352"></a>请求未完成，服务异常。</p>
    </td>
    </tr>
    <tr id="row20561848"><td class="cellrowborder" valign="top" width="61.839999999999996%" headers="mcps1.1.3.1.1 "><p id="p54897010"><a name="p54897010"></a><a name="p54897010"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.16%" headers="mcps1.1.3.1.2 "><p id="p1451523117958"><a name="p1451523117958"></a><a name="p1451523117958"></a>系统暂时不可用，请求受限。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 错误码<a name="section137621219143417"></a>

请参考[返回错误码说明](返回错误码说明.md)。

