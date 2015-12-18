# 获取用户信息
根据uid获取用户信息

- URL：/user/622586376?type=uid

- HTTP请求方式：GET

- 是否登陆：否

- 请求参数：

```
{
   "type":"email"   //in uid,email
}
```

- 返回结果：

```
{
    "meta":{
        "code": 200,
        "message":"OK"
    },
    "data":{
        "uid": 656141312,
        "accout": "",
        "name": "",
        "nickname": "唐启胤",
        "avatar": "http://wx.qlogo.cn/mmopen/Kicho2Jg7kX5wd1XpK7v0guOm9Mn1LYArkWHT5FtBqtvXiaSRic9ngDPZByGicia0z3SaSsxEvkL99NUQ1Xm8bVQAjTjeA9WwGaj3/0",
        "intro": ""
    }
      
}
```

- 关于错误返回值与错误代码，参见 [错误代码说明](../README.md)