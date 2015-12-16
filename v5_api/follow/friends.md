# 获取用户关注列表

- URL：/follow/622586376/friends

- HTTP请求方式：GET

- 是否登陆：否

- 请求参数：

```
{
    "page":1,
    "limit": 10 
      
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
        "friend_uid": 1
        "nickname":"zhanghsan",
        "avatar":"avatar.jpg"
    },
    {
        
        "friend_uid": 2
        "nickname":"zhanghsan",
        "avatar":"avatar.jpg"
    }
    ]   
}
```

- 关于错误返回值与错误代码，参见 [错误代码说明](../README.md)