# articles
博客文章

### 数据结构

```json

{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "aid" : 12345,
    "auto_aid" : 12,
    "user_id" : 52,
    "notebook_id":1, //人个分类
    "title" : "xxx",
    "subtitle":"xxx",
    "summary" : "xxx",
    "body":"xxx",
    "add_time" : 1417663213,
    "update_time" : 1417663213,
    "from":"blogchina",//blogchina|ywt
    "word_count" : 1432,
    
    "pics" : {
        "exists":"y",
        "url":['xxx/1.jpg','xxx/2.jpg'],
    },
    "videos" : {
        "exists":"y",
        "url":['xxx/1.flv','xxx/2.flv'],
    },
    "tag" : ['w3c','nodejs'],
    
    "ip" : "10.10.4.244",
    "last_ip" : "10.10.4.244",
    "state":"a",//a已发布 b草稿箱 c在回收站 d从回收站删除
    "allow":{
        "comment" : "y",
        "reward" : "n",
        "love" : "y",
        "display":"y",//是否允许别人查看
    },
    "monitor" : {
        "is_audit" : "y",
        "is_pending" : "n",
        "is_hidden" : "n",
        "is_del" : "n"
    },
    
}

```