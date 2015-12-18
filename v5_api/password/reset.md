# 找回密码重置密码

- URL：/password/reset

- HTTP请求方式：POST

- 是否登陆：否

- 请求参数：

```
{
    "code":"xxx",
    "password":"123456",
    "password_confirmation" =>"123456",
}
```

- 返回结果：

```
{
    "meta":{
        "code": 200,
        "message":"OK"
    } 
    
}
```

- 关于错误返回值与错误代码，参见 [错误代码说明](../README.md)

