# notifications
通知


### 数据结构
通知的类型有如下几种：

|type|说明|
|:---|:---------|
|follow_user |xxx关注了了您|
|follow_collection |xxx关注了您的专题 《xxx》|
|support_article |xxx喜欢了您的文章  《xxx》|
|comment_article |xxx评论了您的文章  《xxx》|
|collection_new_article |您的专题 《xxx》 有了一篇新投稿|
|collection_new_user |您已成为专题 《xxx》 的编辑|
|collection_invite_user |xxx 邀请您到专题 《xxx》 中投稿 |


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
        "who":123,
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
        "who":123,
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
        "who":123,
        "a_id":234,
        "a_title":"xxx",
    },
    "add_time" : 1450662531,
    "ip" : "127.0.0.1",
    
}


{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "uid" : 597346824,
    "type" : "collection_new_article",
    "data" : {
        "c_id":123,
        "c_name":"xxx",
        
    },
    "add_time" : 1450662531,
    "ip" : "127.0.0.1",
    
}



{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "uid" : 597346824,
    "type" : "collection_new_user",
    "data" : {
        "c_id":123,
        "c_name":"xxx",
        
    },
    "add_time" : 1450662531,
    "ip" : "127.0.0.1",
    
}



{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "uid" : 597346824,
    "type" : "collection_invite_user",
    "data" : {
        "who":123,
        "c_id":234,
        "c_name":"xxx",
        
    },
    "add_time" : 1450662531,
    "ip" : "127.0.0.1",
    
}

```