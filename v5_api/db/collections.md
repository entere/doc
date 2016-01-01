# collections
专题

### 数据结构

```json

{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "cid":123,
    "auto_cid" : 12,
    "user_id" : 52,
    "name" : "xxx",
    "summary" : "xxx",
    "cover":"xxx",//封面
    "color" : "#cccccc",
    "add_time" : 1450668800,
    "update_time" : 1417663213,
    
    "allow_contribute":"Y",//是否允许投稿
    "need_audit":"N",//是否需要审核
    "manager":[1,2,3,4],  
    "state":"A",//用户自己操作A正常 B隐藏 C删除 
    "monitor" : { //监管操作
        "is_hidden" : "N",
        "is_del" : "N"
    },
}

```