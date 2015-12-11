# 队列

开发过程中用到 Redis 实现任务队列，本文档基于laravel5.1

### 注意事项
> * `laravel`关于`queue`配置`'queue'=>'default'` 如果用默认队列名，这个`default`需要重命名，本案中邮件推送到指定队列：`queues:v5:emails`,指定方法：

> * ```php
        $job = (new SendEmail($data))->onQueue('v5:emails');
        $r = $this->dispatch($job);```




> * `redis`队列的监听用如下命令：`php artisan queue:work connection --daemon --sleep=3 --tries=3`  相关参数按实际情况调整;服务端要通过supervisor来监控 以上监听脚本，以实现php脚本挂掉自动重启

> * `job`会被推送到`redis`中，可以在`redis`中通过 `lrange queues:v5:emails 0 10` 命令来查看队列中有那些`job`


### 目前已有的队列：
| key               |  job             | 功能描述 |
| :--------         | :---------       |:----------------|
| queues:v5:emails  | SendEmail      | 发送邮件各种邮件  |