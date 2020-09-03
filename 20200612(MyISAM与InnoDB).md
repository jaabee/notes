[参考链接](https://mp.weixin.qq.com/s?__biz=MjM5ODYxMDA5OQ==&mid=2651961494&idx=1&sn=34f1874c1e36c2bc8ab9f74af6546ec5&chksm=bd2d0d4a8a5a845c566006efce0831e610604a43279aab03e0a6dde9422b63944e908fcc6c05&scene=21#wechat_redirect)
[连接](https://segmentfault.com/a/1190000008227211)

#### 索引 [链接](https://mp.weixin.qq.com/s?__biz=MjM5ODYxMDA5OQ==&mid=2651961494&idx=1&sn=34f1874c1e36c2bc8ab9f74af6546ec5&chksm=bd2d0d4a8a5a845c566006efce0831e610604a43279aab03e0a6dde9422b63944e908fcc6c05&scene=21#wechat_redirect)
> 都是使用B+树
> MyISAM是非聚集索引，索引与行记录是分开存储，叶子节点记录的是数据地址，InnoDB是聚集索引，索引与行记录是存储在一起的，数据记录再叶子节点上
> eg：如果有两个索引id(PK),name(index),select \* from user where name = 'list' 其实会扫描两次索引，一次找到id，一次根据id从聚集索引拿到数据
> mysiam不支持事务，不支持行锁，不支持全文索引，不支持外键，
> mysiam的表行数是存了的，innodb要重新算
> mysiam执行select更快，innodb执行update/insert更快





