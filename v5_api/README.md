# Introduction

v5_api 错误码规范

    200 没有错误
    400 参数错误
    409 已存在，重复操作
    404 不存在（用户不存在，单个不存在）
    500 数据库写动作异常（更新，修改，删除），可能唯一键重复
    401 认证失败(登录、token、签名等)
    503 服务器异常
    408 超时