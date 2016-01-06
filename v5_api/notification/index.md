# 获取用户提醒列表

- URL：/notification

- HTTP请求方式：GET

- 是否登陆：是

- 请求参数：

```

curl -X GET \
    /url \
    -H "Authorization: bearer token"

{
    "unread":"y",
}

```

- 返回结果：

```
{
    "meta":{
        "code": 200,
        "message":"OK"
    },
    "data": [
    {
        "uid" : 597346824,
        "type" : "follow_collection",
        "data" : {
            "who":123,
            "c_id":234,
            "c_name":"xxx",
        },
        "add_time" : 1450662531,
        "unread":"y",//"y|n"
        
    },
    {
        "_id" : ObjectId("547fd2ed2997cfa475516662"),
        "uid" : 597346824,
        "type" : "follow_user",
        "data" : {
            "who":123,
        },
        "add_time" : 1450662531,
        "unread":"n",//"y|n"
        
    }
    ]   
}

```

- 关于错误返回值与错误代码，参见 [错误代码说明](../README.md)