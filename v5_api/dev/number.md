# 统计数量
说明：article:文章数量

### 用户各数量 redis hash

```

['v5:num:uid:1'=>
    [
       'uid'=>'1',
       'click'=>'33',
       'support'=>'2',
       'oppose'=>'3',
       'comment'=>'6'
       'fans'=>'22',//粉丝数
       'friends'=>'4',//偶像数
       'article'=>'',
    ]
]

```

### 文章各数量 redis hash

```

['v5:num:aid:12'=>
    [
       'aid'=>'1',
       'click'=>'33',
       'support'=>'2',
       'oppose'=>'3',
       'comment'=>'6',
    ]
]

```

### 个人分类各数量 redis hash

```

['v5:num:nid:12'=>
    [
       'nid'=>'1',
       'fans'=>'22',
       'article'=>'33',
       
    ]
]

```


### 专题各数量 redis hash

```

['v5:num:cid:12'=>
    [
       'cid'=>'1',
       'fans'=>'22',
       'article'=>'33',
       
    ]
]

```