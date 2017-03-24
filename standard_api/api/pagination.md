# 分页数据

### JSON
##### 参考
```
{
    "meta": {
        "code": "value",   //结果码，必需
        "message": "value"
    },
    "page": {    //分页参数，必需。
        "limit":"value",    //每页记录条数
        "page": "value",    //本页页码
        "count": "value" //总记录数
    },
    "data": [{//列表数据，数组
    },{
    }]
}
```
##### 示例
```
{

    "meta": {
        "code": 200, 
        "message": "success"
    },
    "page": {    //分页参数，必需。
        "limit":"20",    //每页记录条数
        "page": "1",    //本页页码
        "count": "200" //总记录数
    },
    "data": [{
        "id":1,
        "title":"每天五分钟，给思想加油",
        "content": "博客中国是中国博客的发源地，自媒体意见领袖在根据地",
        "created_at": "Fri Aug 22 00:00:00 +0800 2014"
     },{
        "id":2,
        "title":"胡适“回家”干什么",
        "content": "设若地下有知，我们再去问一问这位适之先生",
        "created_at": "Fri Aug 21 00:00:00 +0800 2014"
        
     }]
}
```

### XML
##### 参考
```
<?xml version="1.0" encoding="utf-8"?> 
<result>
    <meta>
        <code></code>
        <message></message>
    </meta>
    <page>
        <limit></limit>
        <page></page>
        <count></count>
    </page>
    <data>
        <data>
            <id></id>
            <title></title>
            <content></content>
            <created_at></created_at>
        </data>
        <data>
            <id></id>
            <title></title>
            <content></content>
            <created_at></created_at>
        </data>
    </data>
</result>
```
##### 示例

```
<?xml version="1.0" encoding="utf-8"?> 
<result>
    <meta>
        <code>200</code>
        <message>success</message>
    </meta>
    <page>
        <limit>20</limit>
        <page>1</page>
        <count>200</count>
    </page>
    <data>
        <data>
            <id>1</id>
            <title>每天五分钟，给思想加油</title>
            <content>博客中国是中国博客的发源地，自媒体意见领袖在根据地</content>
            <created_at>Fri Aug 22 00:00:00 +0800 2014</created_at>
        </data>
        <data>
            <id>2</id>
            <title>胡适“回家”干什么</title>
            <content>设若地下有知，我们再去问一问这位适之先生地</content>
            <created_at>Fri Aug 21 00:00:00 +0800 2014</created_at>
        </data>
    </data>
</result>
```