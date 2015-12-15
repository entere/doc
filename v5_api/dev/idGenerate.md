# idGenerate

用户`id`生成规则：`redis`产生自增`id`,`key`为`v5:auto:uid`，拿到自增`id`后，根据`SequenceNumber::generateNumber($autoUid,$prefix='',$width=9)`方法生成一个等宽随机`uid`

### `autoid`在`redis`中的示例：

| key               |  value        |  描述 |
| :--------         | :---------       |:----------------|
| v5:auto:uid        | 27     | 自增uid        |



### 查看 `v5:auto:uid`

```
get v5:auto:uid

```




