# 测试接口


<a name="overview"></a>
## Overview
更多Spring Boot相关文章请关注


### Version information
*Version* : 1.0


### Contact information
*Contact* : 久而久之


### License information
*Terms of service* : http://blog.didispace.com/


### URI scheme
*Host* : localhost:8060  
*BasePath* : /


### Tags

* async-controller : Async Controller
* file-controller : File Controller
* user-controller : User Controller




<a name="paths"></a>
## Paths

<a name="uploadusingpost"></a>
### upload
```
POST /file
```


#### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**FormData**|**file**  <br>*optional*|file|file|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[FileInfo](#fileinfo)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `multipart/form-data`


#### Produces

* `*/*`


#### Tags

* file-controller


<a name="downloadusingget"></a>
### download
```
GET /file/{id}
```


#### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|string|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* file-controller


<a name="orderusingpost"></a>
### order
```
POST /order
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[DeferredResult«string»](#54d560f964f28522b9d967755e16a73a)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* async-controller


<a name="orderusingget"></a>
### order
```
GET /order
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[DeferredResult«string»](#54d560f964f28522b9d967755e16a73a)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* async-controller


<a name="orderusingput"></a>
### order
```
PUT /order
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[DeferredResult«string»](#54d560f964f28522b9d967755e16a73a)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* async-controller


<a name="orderusingdelete"></a>
### order
```
DELETE /order
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[DeferredResult«string»](#54d560f964f28522b9d967755e16a73a)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* async-controller


<a name="orderusingpatch"></a>
### order
```
PATCH /order
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[DeferredResult«string»](#54d560f964f28522b9d967755e16a73a)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* async-controller


<a name="orderusinghead"></a>
### order
```
HEAD /order
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[DeferredResult«string»](#54d560f964f28522b9d967755e16a73a)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* async-controller


<a name="orderusingoptions"></a>
### order
```
OPTIONS /order
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[DeferredResult«string»](#54d560f964f28522b9d967755e16a73a)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* async-controller


<a name="createusingpost"></a>
### 创建用户
```
POST /user
```


#### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**user**  <br>*required*|user|[User](#user)|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[User](#user)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* user-controller


<a name="queryusingget"></a>
### 用户查询服务
```
GET /user
```


#### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Query**|**age**  <br>*optional*|用户年龄起始值|integer (int32)|
|**Query**|**ageTo**  <br>*optional*|用户年龄终止值|integer (int32)|
|**Query**|**username**  <br>*optional*||string|
|**Query**|**xxx**  <br>*optional*||string|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|< [User](#user) > array|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* user-controller


<a name="getinfousingget"></a>
### getInfo
```
GET /user/{id}
```


#### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*optional*|用户id|string|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[User](#user)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* user-controller


<a name="updateusingput"></a>
### update
```
PUT /user/{id}
```


#### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**user**  <br>*required*|user|[User](#user)|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[User](#user)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* user-controller


<a name="deleteusingdelete"></a>
### 删除用户
```
DELETE /user/{id}
```


#### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|string|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|No Content|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


#### Consumes

* `application/json`


#### Produces

* `*/*`


#### Tags

* user-controller




<a name="definitions"></a>
## Definitions

<a name="54d560f964f28522b9d967755e16a73a"></a>
### DeferredResult«string»

|Name|Schema|
|---|---|
|**result**  <br>*optional*|object|
|**setOrExpired**  <br>*optional*|boolean|


<a name="fileinfo"></a>
### FileInfo

|Name|Schema|
|---|---|
|**path**  <br>*optional*|string|


<a name="user"></a>
### User

|Name|Description|Schema|
|---|---|---|
|**birthday**  <br>*optional*||string (date-time)|
|**id**  <br>*optional*||string|
|**password**  <br>*optional*||string|
|**username**  <br>*optional*|用户名|string|





