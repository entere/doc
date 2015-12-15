# 登录

- URL：/sign/in 

- HTTP请求方式：POST

- 是否登陆：否

- 请求参数：

```
{
    "accout": "entere@126.com", 
    "password": "111111",  
}
```

- 返回结果：

```
{
    "meta":{
        "code": 200,   //结果码，必需。客户端应首先根据此项结果进行相应处理。
        "message":"OK"
    },
    "data": {
        "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOjE0NDY4MDI0MjcsImV4cCI6MTQ0NjgwNjI1NSwiaWF0IjoxNDQ2ODA1NjU1LCJqdGkiOiIxNDQ2ODA1NjU1MzEwNSIsImRhdGEiOnsidWlkIjoxNDQ2ODAyNDI3fX0.qQC-Dom8_HVXGnX8ZqltGoZaSaZmX9NHFGmBE9dDjUk"
    }
    
}
```


