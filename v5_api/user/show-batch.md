# 批量获取用户信息
根据uids获取用户信息


- URL：/user/batch

- HTTP请求方式：GET

- 是否登陆：否

- 请求参数：

```
{
   "uids":"505072640,521849856" 
}
```

- 返回结果：/user/batch?uids=505072640,521849856

```
{
    "meta":{
        "code": 200,
        "message":"OK"
    },
    "data":{
        "505072640": {
            "uid": 505072640,
            "accout": "13141223060",
            "nickname": "qiyin",
            "avatar": "avatar.jpg",
            "add_time": 1452168609,
            "intro": "",
            "homepage": "",
            "email": "",
            "name": ""
        },
        "521849856": {
            "uid": 521849856,
            "accout": "crabhw@qq.com",
            "nickname": "crabhw",
            "avatar": "avatar.jpg",
            "add_time": 1451698242,
            "intro": "",
            "homepage": "",
            "email": "crabhw@qq.com",
            "name": ""
        }
    }
      
}
```


- 关于错误返回值与错误代码，参见 [错误代码说明](../README.md)