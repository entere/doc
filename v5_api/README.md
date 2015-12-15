# Introduction

### `v5_api` 错误码规范


|code|message                 |说明|
|:---|:---------              |:-----------------------|
|200 |OK                      |操作成功(login success……) |
|400 |Bad Request             |参数错误，错误的请求 |
|401 |Unauthorized            |认证失败(登录、token、签名等) |
|404 |Not Found               |不存在（数据库查询不到） |
|408 |Request Time-out        |超时 |
|409 |Conflict                |冲突，已存在，重复操作 |
|500 |Internal Server Error   |服务器内部错误，数据库异常，键重复 |
|503 |Service Unavailable     |服务器异常 |


### `v5_api`域名
http://api5.blogcore.cn


