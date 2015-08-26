# 消息通知流程

### 1.概述

以用户A向用户B发通知为例

A向B发通知，系统先判断B有没有在线，如果B不在线，通知存下来，暂不发送

B在线分几种情况：web在线（chrome在线、safari在线），移动在线；如果果同时在线，通知都要推送到

B退出也分几种情况：比如B只退出的chrome,safari还登录着，清理在线时就是区分对待了

### 2.数据结构
用redis来存储 用户id(uid),socketid(sid),channelid(cid)之前的关系
解解释一下这uid,cid和sid

>uid:登陆用户的唯一id
>cid:用户在safari上登陆和在chrome上登陆是不一样的，cid的值可以是sessionid,因为每次登录产生的sessionid都不一样，也可以是其它比如 uid.microtime(true),此文档约定其格式为:33.1440575849.7297
>sid:socketid

数结结构示范

```
smembers msg_uid:33
1) "33.1440577128.5168"
2) "33.1440575849.7297"


smembers msg_cid:33.1440577128.5168
1) "307"
2) "309"

smembers msg_cid:33.1440575849.7297
1) "305"
2) "306"
```











