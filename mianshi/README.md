### 计算机网络
1. HTTP和HTTPS
2. TCP和UDP
3. Cookie和Session
4. TCP三次握手，四次挥手

### 数据库
1. redis数据类型

五种：string、hash、list、set、zset

2. redis持久化

分别是RDB(RedisDataBase)和AOF(AppendOnlyFile)

RDB(RedisDataBase)代表快照模式，容易造成数据丢失

AOF(AppendOnlyFile)一般用在秒杀场景，必须保证下单的信息不被丢失

3. mybatis一级缓存、二级缓存



4. MySQL数据库索引讲一下

索引是一种特殊的文件（innodb数据表上的索引是表空间的一个组成部分），它们包含着对数据表里所有记录的引用指针。

更通俗的说，数据库索引就好比是一本书前面的目录，能加快数据库的查询速度。

5. MySQL数据库锁
6. MySQL引擎

MyISAM和InnoDB。
MyISAM不支持行级锁，外键，事务
InnoDB支持行级锁，外键，事务

7. 乐观锁实现

查询时不加锁，更新数据库时判断。

### JAVA
1. 继承、重载、重写

继承：子类共性抽取形成父类（接口），重载：方法名+方法参数相同，重写：多态针对的是重写

2. Java里的LinkedList和LinkedHashMap有啥区别
3. LinkedHashMap和HashMap有啥区别
4. GC知道吗，聊一聊GC的流程
5. Java内存模型整一下
6. 线程安全问题
7. HashMap是线程安全吗？介绍一个线程安全的集合类？
8. 设计模式
9. 反射
10. Linux命令：查看CPU、查看内存、查看端口占用
11. 介绍一下你知道的排序和时间复杂度。
12. 手撕快排


### 框架
1. SpringBean的初始化
2. SpringMVC的请求流程
3. SpringIOC和AOP
4. Elasticsearch的倒排索引
5. RabbitMQ的各种模式
