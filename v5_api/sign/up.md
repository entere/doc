# 注册

- URL：/sign/up 

- HTTP请求方式：POST

- 是否登陆：否

- 请求参数：

```
{
    "accout": "entere@126.com", 
    "password": "xxxxxx",  
    "nickname": "entere",
    "reg_from": "blogchina",
    
    "openid" : "",
    "register_ip":"10.10.3.212"
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
        "uid":324564345,
        "accout":"entere@126.com",
        "nickname":"entere"
    }
    
}
```

- 关于错误返回值与错误代码，参见 [错误代码说明](../README.md)



