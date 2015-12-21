# jwt

用户登录时会产生`json web token`,`jwt`存在`redis`中,有过期时间，`jwt`是验证用户是否登录的令牌，也是检验是否有`api`权限的标识


### `jwt`在`redis`中的示例：

| key               |  value        |  描述 |
| :--------         | :---------       |:----------------|
| v5:jwt:uid:505146376:iat:1450082539  | jwt字串      | 用户每次登录都会产生不同的jwt,多终端退出登录互不影响 set类型  |
| v5:jwt:md5:AFEB0549A6B245B52D7D55E7C7D919A0 | uid和过期时间   | 退出登陆会清理此key hash类型 |

### `redis`中查看示例：

```
get v5:jwt:uid:505146376:iat:1450082539
"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOjYwNTczNTQzMiwiZXhwIjoxNDUxMDI5NTc4LCJpYXQiOjE0NTA2Njk1NzgsImp0aSI6IjE0NTA2Njk1Nzg4NTM4IiwiZGF0YSI6eyJ1aWQiOjYwNTczNTQzMn19.OClfCMm8IqkKWVDcaTQZDghBu0XVLQ5aSqRJqazatZ8"

hgetall v5:jwt:md5:AFEB0549A6B245B52D7D55E7C7D919A0
1) "uid"
2) "505146376"
3) "iat"
4) "1450082539"
```