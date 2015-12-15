# 关注

- URL：/follow 

- HTTP请求方式：POST

- 是否登陆：是

- 请求参数：

```
{
    "token":"xxxxx"
    "friend_uid": 132432234, 
    "ip": "113.123.211.122",  
}
```

- 返回结果：

```
{
    "meta":{
        "code": 200,
        "message":"OK"
    },
    "data": {
        "fans_uid": 622586376,
        "friend_uid": 132432234
    }
    
}
```
