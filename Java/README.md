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
10. 介绍一下你知道的排序和时间复杂度。
11. 手撕快排


### 计算机网络
1. HTTP和HTTPS
2. TCP和UDP
3. Cookie和Session
4. TCP三次握手，四次挥手

### 操作系统
1. Linux命令：查看CPU、查看内存、查看端口占用

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

### 常用框架
1. SpringBean的初始化
2. SpringMVC的请求流程
3. SpringIOC和AOP

### 认证授权（JWT、SSO）

### 分布式
4. Elasticsearch的倒排索引
5. RabbitMQ的各种模式

### 大型网站架构
1. 性能测试
2. 高并发
3.高可用

### 微服务
1. Spring Cloud

### String能被继承吗？为什么？
不可以，因为String类有final修饰符，而final不能被继承的，实现细节不允许改变。平常我们定义的String str = " a ";其实和String str = new String("a");还是有差异的。

前者默认调用的String.valueof来返回String的实例对象，至于调用哪个则取决于你的赋值，比如String num = 1;调用的是public static String valueOf(int i){

   return Integer.toString(i);

}

后者则是调用如下部分:

public String(String original) { 
this.value = original.value; 
this.hash = original.hash; 
} 

最后我们的变量都存储在一个char数组中。

private final char value[];

2、数据库索引

3、接口和抽象类有什么区别

4、Java中的集合类（容器类）

### ArrayList 和 LinkedList 有什么区别。

ArrayList和LinkedList都实现了List接口，有以下的不同点： 

1.ArrayList是基于索引的数据接口。它的底层是数组。它可以以O(1)时间复杂度对元素进行随机访问。以此对应，LinkedList是以元素列表的形式存储的数据，每一个元素都和它的前一个后一个元素链接在一起，在这种情况下，查找某个元素的时间复杂度是O(n)。 

2.相对于ArrayList，LinkedList的插入，添加，删除操作速度更快，因为当元素被添加到集合任意位置的时候，不需要像数组那样重新计算大小或者是更新索引。

3.LinkedList比ArrayList更占内存，因为LinkedList为每一个节点存储了两个引用，一个指向前一个元素，一个指向下一个元素。

 

5、HashMap & HashTable

### String， Stringbuffer， StringBuilder 的区别。

String 字符串常量(final修饰，不可被继承)，String是常量，当创建之后即不能更改。(可以通过StringBuffer和StringBuilder创建String对象(常用的两个字符串操作类)。) 

StringBuffer 字符串变量（线程安全）,其也是final类别的，不允许被继承，其中的绝大多数方法都进行了同步处理，包括常用的Append方法也做了同步处理。其自jdk1.0起就已经出现。其toString方法会进行对象缓存，以减少元素的复制开销。

public synchronized String toString() { 
if (toStringCache == null) { 
toStringCache = Arrays.copyOfRange(value, 0, count); 
} 
return new String(toStringCache, true); 
}

StringBuilder 字符串变量，（非线程安全）其自jdk1.5起开始出现。与StringBuffer一样都继承和实现同一个接口和类，方法除了没有使用synch修饰以外基本一致，不同之处在于最后toString的时候，会直接返回一个新对象。

public String toString() { 
// Create a copy, don’t share the array 
return new String(value, 0, count); 
}

7、创建线程的方法

8、如何实现线程同步

9、运行时异常

10、数据库优化

11、spring框架（IOC、AOP）

12、页面加载缓慢的原因，解决方法

13、存储引擎

14、statement & preparedstatement

[「Java学习+面试指南」一份涵盖大部分Java程序员所需要掌握的核心知识。 ](https://github.com/Snailclimb/JavaGuide#%E5%9F%BA%E7%A1%80)

