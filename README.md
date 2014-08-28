JgFramework
===========

基于Netty的强大的游戏服务器框架

特点
===
~~~
1、使用netty作为底层，性能得到保障
2、支持socket和websocket2种连接模式，可以自由选择
3、简单实用的路由，方便handler开发
4、异步无锁的数据同步
5、spring+Hibernia的自动注入和事务管理
6、mysql数据库的读写分离以及对多数据库的读写支持
7、传输数据的多样化，可以自用实现接口来实现不同的传输数据类型，现在使用的是json
8、框架自带了认证服务和管理服务，有简单的管理命令，需要telnet连接到端口（默认38080）
9、方便的ip段限制功能
10、方便设置心跳检查
11、登录方和服务端之间的认证，可通过实际接口来完成，默认使用的rsa加密传输认证码
12、性能优良的排队系统
13、丰富的工具类：memcache、redis等
14、基本游戏模块的抽象
~~~

性能测试
======
##### *测试信息*
~~~
cpu : AMD A10
内存 : 8G
测试脚本 : src/test/java/client/TestWebSocket.java
测试方式 : 自压
~~~
##### *测试结果*
~~~
在100个登录用户，每个用户在登录完成，再init操作之后，每个用户发送100000个请求，   
得到每秒处理请求数在3.5W左右。
~~~

欢迎加入
======
如果对该系统有兴趣可以发邮件至 bupt1987@gmail.com 一起探讨，欢迎加入


例子
===
见：https://github.com/bupt1987/JgWeb
