# 验证邮箱发送邮件
邮箱不存在，code返回404

- URL：/setting/email/confirm

- HTTP请求方式：POST

- 是否登陆：否

- 请求参数：

```
{
    "email":"xxxxx"
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