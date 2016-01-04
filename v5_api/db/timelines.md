# timelines
我的动态


### 数据结构
动态的类型有如下几种：

|type|说明|
|:---|:---------|
|follow_user |我 关注了作家 xxx|
|follow_collection |我 关注了专题 xxx|
|support_article |我 喜欢了文章  xxx|
|comment_article |我 评论了文章  xxx|
|sign_up |我 加入了博客中国|


各类型数据结构：

```json

{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "uid" : 597346824,
    "type" : "follow_user",
    "data" : {
        "who":123,
    },
    "add_time" : 1450662531,
    "ip" : "127.0.0.1",
    
}


{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "uid" : 597346824,
    "type" : "follow_collection",
    "data" : {
        "c_id":234,
        "c_name":"xxx",
    },
    "add_time" : 1450662531,
    "ip" : "127.0.0.1",
    
}



{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "uid" : 597346824,
    "type" : "support_article",
    "data" : {
        "a_id":234,
        "a_title":"xxx",
    },
    "add_time" : 1450662531,
    "ip" : "127.0.0.1",
    
}



{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "uid" : 597346824,
    "type" : "comment_article",
    "data" : {
        "a_id":234,
        "a_title":"xxx",
        "comment":"xxx",
    },
    "add_time" : 1450662531,
    "ip" : "127.0.0.1",
    
}



{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "uid" : 597346824,
    "type" : "sign_up",
    "add_time" : 1450662531,
    "ip" : "127.0.0.1",
    
}

```