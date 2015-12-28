# articles

### 数据结构

```json

{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "aid" : 12345,
    "user_id" : 52,
    "notebook_id":1, //人个分类
    "title" : "xxx",
    "subtitle":"xxx",
    "summary" : "xxx",
    "body":"xxx",
    "pubdate" : 1417663213,
    "uppdate" : 1417663213,
    "from":"blogchina",//blogchina|ywt
    "word_count" : 1432,
    
    "pics" : {
        "exists":"Y",
        "url":['xxx/1.jpg','xxx/2.jpg'],
    },
    "videos" : {
        "exists":"Y",
        "url":['xxx/1.flv','xxx/2.flv'],
    },
    "tag" : [],
    
    "ip" : "10.10.4.244",
    "last_ip" : "10.10.4.244",
    "state":"A",//A已发布 B草稿箱 C在回收站 D从回收站删除
    "allow":{
        "comment" : "Y",
        "reward" : "N",
        "love" : "Y",
    },
    "monitor" : {
        "is_audit" : "Y",
        "is_pending" : "N",
        "is_hidden" : "N",
        "is_del" : "N"
    },
    
}

```