# 1.登录

### 1.1 登录

- URL：/sign/in 

- HTTP请求方式：POST

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
        "code": "200",   //结果码，必需。客户端应首先根据此项结果进行相应处理。
        "message":"login success"
    },
    "data": {
        "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOjE0NDY4MDI0MjcsImV4cCI6MTQ0NjgwNjI1NSwiaWF0IjoxNDQ2ODA1NjU1LCJqdGkiOiIxNDQ2ODA1NjU1MzEwNSIsImRhdGEiOnsidWlkIjoxNDQ2ODAyNDI3fX0.qQC-Dom8_HVXGnX8ZqltGoZaSaZmX9NHFGmBE9dDjUk"
    }
    
}
```

### 1.2 退出

- URL：/sign/out

- HTTP请求方式：GET

- 请求参数：

```
{
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOjE0NDY4MDI0MjcsImV4cCI6MTQ0NjgwNjI1NSwiaWF0IjoxNDQ2ODA1NjU1LCJqdGkiOiIxNDQ2ODA1NjU1MzEwNSIsImRhdGEiOnsidWlkIjoxNDQ2ODAyNDI3fX0.qQC-Dom8_HVXGnX8ZqltGoZaSaZmX9NHFGmBE9dDjUk", 
      
}
```

- 返回结果：

```
{
    "meta":{
        "code": "200",   //结果码，必需。客户端应首先根据此项结果进行相应处理。
        "message":"logout success"
    }
    
}
```
