# 查询API所有版本<a name="ZH-CN_TOPIC_0171212585"></a>

## 功能介绍<a name="section66578044"></a>

查询云监控支持的API所有版本号。

## URI<a name="section62331491"></a>

GET /

## 请求消息<a name="section24112512"></a>

请求样例

```
GET https://{Cloud Eye的endpoint}/
```

## 响应消息<a name="section15686020"></a>

-   响应参数

    **表 1**  要素说明

    <a name="table26246518152631"></a>
    <table><thead align="left"><tr id="row29602547152631"><th class="cellrowborder" valign="top" width="17.61%" id="mcps1.2.4.1.1"><p id="p1143665616354"><a name="p1143665616354"></a><a name="p1143665616354"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.23%" id="mcps1.2.4.1.2"><p id="p11440156143517"><a name="p11440156143517"></a><a name="p11440156143517"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="64.16%" id="mcps1.2.4.1.3"><p id="p244212561357"><a name="p244212561357"></a><a name="p244212561357"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row56174697152631"><td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.4.1.1 "><p id="p4445556153516"><a name="p4445556153516"></a><a name="p4445556153516"></a>versions</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.2 "><p id="p444855610353"><a name="p444855610353"></a><a name="p444855610353"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.16%" headers="mcps1.2.4.1.3 "><p id="p344911569354"><a name="p344911569354"></a><a name="p344911569354"></a>描述version相关对象的列表。</p>
    <p id="p76411522123610"><a name="p76411522123610"></a><a name="p76411522123610"></a>详细参数说明请参见<a href="#table11622191810339">表2</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  versions字段数据结构说明

    <a name="table11622191810339"></a>
    <table><thead align="left"><tr id="row4619181833318"><th class="cellrowborder" valign="top" width="17.61%" id="mcps1.2.4.1.1"><p id="p8618218183315"><a name="p8618218183315"></a><a name="p8618218183315"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.23%" id="mcps1.2.4.1.2"><p id="p46182182336"><a name="p46182182336"></a><a name="p46182182336"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="64.16%" id="mcps1.2.4.1.3"><p id="p1361819181337"><a name="p1361819181337"></a><a name="p1361819181337"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1261921810335"><td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.4.1.1 "><p id="p1619718203313"><a name="p1619718203313"></a><a name="p1619718203313"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.2 "><p id="p186194185335"><a name="p186194185335"></a><a name="p186194185335"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.16%" headers="mcps1.2.4.1.3 "><p id="p8619418123311"><a name="p8619418123311"></a><a name="p8619418123311"></a>版本ID（版本号），如v1。</p>
    </td>
    </tr>
    <tr id="row106201018103311"><td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.4.1.1 "><p id="p12620181823313"><a name="p12620181823313"></a><a name="p12620181823313"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.2 "><p id="p12620171823314"><a name="p12620171823314"></a><a name="p12620171823314"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.16%" headers="mcps1.2.4.1.3 "><p id="p46207186338"><a name="p46207186338"></a><a name="p46207186338"></a>API的URL地址。</p>
    <p id="p551085418378"><a name="p551085418378"></a><a name="p551085418378"></a>详细参数说明请参见<a href="#table7157926103418">表3</a>。</p>
    </td>
    </tr>
    <tr id="row186211518163313"><td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.4.1.1 "><p id="p1562111184330"><a name="p1562111184330"></a><a name="p1562111184330"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.2 "><p id="p762171863315"><a name="p762171863315"></a><a name="p762171863315"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.16%" headers="mcps1.2.4.1.3 "><p id="p196210182338"><a name="p196210182338"></a><a name="p196210182338"></a>若该版本API支持微版本，该参数表示支持的最大微版本号，如果不支持微版本，则为空。</p>
    </td>
    </tr>
    <tr id="row862171813317"><td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.4.1.1 "><p id="p262191883312"><a name="p262191883312"></a><a name="p262191883312"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.2 "><p id="p20621118153312"><a name="p20621118153312"></a><a name="p20621118153312"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.16%" headers="mcps1.2.4.1.3 "><p id="p362121813335"><a name="p362121813335"></a><a name="p362121813335"></a>版本状态，为如下3种：</p>
    <p id="p10621201813316"><a name="p10621201813316"></a><a name="p10621201813316"></a>CURRENT：表示该版本为主推版本。</p>
    <p id="p662112186338"><a name="p662112186338"></a><a name="p662112186338"></a>SUPPORTED：表示为老版本，但是现在还继续支持。</p>
    <p id="p18621141813331"><a name="p18621141813331"></a><a name="p18621141813331"></a>DEPRECATED：表示为废弃版本，存在后续删除的可能。</p>
    </td>
    </tr>
    <tr id="row16223181336"><td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.4.1.1 "><p id="p1062261817332"><a name="p1062261817332"></a><a name="p1062261817332"></a>updated</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.2 "><p id="p16228184334"><a name="p16228184334"></a><a name="p16228184334"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.16%" headers="mcps1.2.4.1.3 "><p id="p56220183330"><a name="p56220183330"></a><a name="p56220183330"></a>版本发布时间，采用UTC时间表示。如v1发布的时间2014-06-28T12:20:21Z。</p>
    </td>
    </tr>
    <tr id="row206221018163316"><td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.4.1.1 "><p id="p8622171816333"><a name="p8622171816333"></a><a name="p8622171816333"></a>min_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.2 "><p id="p4622121819338"><a name="p4622121819338"></a><a name="p4622121819338"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.16%" headers="mcps1.2.4.1.3 "><p id="p16221118103315"><a name="p16221118103315"></a><a name="p16221118103315"></a>若该版本API 支持微版本，该参数表示支持的最小微版本号， 如果不支持微版本，则为空。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  links字段数据结构说明

    <a name="table7157926103418"></a>
    <table><thead align="left"><tr id="row6157112653419"><th class="cellrowborder" valign="top" width="17.61%" id="mcps1.2.4.1.1"><p id="p1515711268345"><a name="p1515711268345"></a><a name="p1515711268345"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.23%" id="mcps1.2.4.1.2"><p id="p4157192614343"><a name="p4157192614343"></a><a name="p4157192614343"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="64.16%" id="mcps1.2.4.1.3"><p id="p7157102613346"><a name="p7157102613346"></a><a name="p7157102613346"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1915852612341"><td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.4.1.1 "><p id="p1515872614346"><a name="p1515872614346"></a><a name="p1515872614346"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.2 "><p id="p2158162616349"><a name="p2158162616349"></a><a name="p2158162616349"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.16%" headers="mcps1.2.4.1.3 "><p id="p615813265341"><a name="p615813265341"></a><a name="p615813265341"></a>当前API版本的引用地址。</p>
    </td>
    </tr>
    <tr id="row1158182615345"><td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.4.1.1 "><p id="p4158162633414"><a name="p4158162633414"></a><a name="p4158162633414"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.2 "><p id="p191584262345"><a name="p191584262345"></a><a name="p191584262345"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.16%" headers="mcps1.2.4.1.3 "><p id="p4158182603413"><a name="p4158182603413"></a><a name="p4158182603413"></a>当前API版本和被引用地址的关系。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
      "versions": [
        {
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
      ]
    }
    ```


## 返回值<a name="section6956456"></a>

-   正常

    200

-   异常

    <a name="table46793998"></a>
    <table><thead align="left"><tr id="row65573909"><th class="cellrowborder" valign="top" width="35.120000000000005%" id="mcps1.1.3.1.1"><p id="p9886408"><a name="p9886408"></a><a name="p9886408"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="64.88000000000001%" id="mcps1.1.3.1.2"><p id="p62601592"><a name="p62601592"></a><a name="p62601592"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row37564172"><td class="cellrowborder" valign="top" width="35.120000000000005%" headers="mcps1.1.3.1.1 "><p id="p22799085"><a name="p22799085"></a><a name="p22799085"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.1.3.1.2 "><p id="p44643603"><a name="p44643603"></a><a name="p44643603"></a>请求错误。</p>
    </td>
    </tr>
    <tr id="row66248115"><td class="cellrowborder" valign="top" width="35.120000000000005%" headers="mcps1.1.3.1.1 "><p id="p64497130"><a name="p64497130"></a><a name="p64497130"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.1.3.1.2 "><p id="p42202994"><a name="p42202994"></a><a name="p42202994"></a>未提供认证信息，或认证信息错误。</p>
    </td>
    </tr>
    <tr id="row44282627"><td class="cellrowborder" valign="top" width="35.120000000000005%" headers="mcps1.1.3.1.1 "><p id="p30123063"><a name="p30123063"></a><a name="p30123063"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.1.3.1.2 "><p id="p15114764"><a name="p15114764"></a><a name="p15114764"></a>请求页面被禁止访问。</p>
    </td>
    </tr>
    <tr id="row1815156"><td class="cellrowborder" valign="top" width="35.120000000000005%" headers="mcps1.1.3.1.1 "><p id="p12809933"><a name="p12809933"></a><a name="p12809933"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.1.3.1.2 "><p id="p10309404"><a name="p10309404"></a><a name="p10309404"></a>请求超出了服务器的等待时间。</p>
    </td>
    </tr>
    <tr id="row25675773"><td class="cellrowborder" valign="top" width="35.120000000000005%" headers="mcps1.1.3.1.1 "><p id="p66471715"><a name="p66471715"></a><a name="p66471715"></a>429 Too Many Requests</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.1.3.1.2 "><p id="p5281111"><a name="p5281111"></a><a name="p5281111"></a>当前请求过多。</p>
    </td>
    </tr>
    <tr id="row47530006"><td class="cellrowborder" valign="top" width="35.120000000000005%" headers="mcps1.1.3.1.1 "><p id="p24725298"><a name="p24725298"></a><a name="p24725298"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.1.3.1.2 "><p id="p39567352"><a name="p39567352"></a><a name="p39567352"></a>请求未完成，服务异常。</p>
    </td>
    </tr>
    <tr id="row20561848"><td class="cellrowborder" valign="top" width="35.120000000000005%" headers="mcps1.1.3.1.1 "><p id="p54897010"><a name="p54897010"></a><a name="p54897010"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.1.3.1.2 "><p id="p1451523117958"><a name="p1451523117958"></a><a name="p1451523117958"></a>系统暂时不可用，请求受限。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 错误码<a name="section137621219143417"></a>

请参考[返回错误码说明](返回错误码说明.md)。

