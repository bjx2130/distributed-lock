# distributed-lock
分布式锁

现在面试都会聊聊分布式系统，通常面试官都会从服务框架（Spring Cloud、Dubbo），一路聊到分布式事务、分布式锁、ZooKeeper等知识。今天就来聊聊分布式锁这块的知识，先具体的来看看Redis分布式锁的实现原理。



如果在公司里落地生产环境用分布式锁的时候，一定是会用开源类库的，比如Redis分布式锁，一般就是用Redisson框架就好了，非常的简便易用。感兴趣可以去Redisson官网看看如何在项目中引入Redisson的依赖，然后基于Redis实现分布式锁的加锁与释放锁。



一段简单的使用代码片段，先直观的感受一下：

![login](https://github.com/github用户名/项目名称/raw/master[分支名称]/screenshots/login.png)

是不是感觉简单的不行！此外，还支持Redis单实例、Redis哨兵、Redis Cluster、redis master-slave等各种部署架构，都可以完美实现。


