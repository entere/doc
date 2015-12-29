# footprints
最新来访问，脚印

### 数据结构

```json

{
    "_id" : ObjectId("547fd2ed2997cfa475516662"),
    "fid":"xxx"
    "user_id" : 52,
    "to_user_id":54,//访问了谁
    "add_time" : 1417663213,
    "total":20,//同一人多次访问,访问数+1
    "state":"A",//用户自己操作A正常 B隐藏 C删除 
    "monitor" : { //监管操作
        "is_hidden" : "N",
        "is_del" : "N"
    },
    
}

```