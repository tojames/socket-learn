# socket-learn
Socket网络编程(java语言实现)

本项目主要是介绍了socket的使用和NIO的使用

工具:idea,maven

用一些实战例子结合介绍，如:聊天室

# 版本v0.2.3
在这个版本中,优化了读线程的数量,把服务器接受到的消息封装到一个任务里,交给线程池异步去执行

当然,在socket接收数据的时候也是采用了无阻塞的NIO模式,采用异步加回调的方式完成这部分的操作

在这个版本中,无法解决消息粘包,消息丢包等问题.

服务器执行流程如下:

![image](https://github.com/13days/socket-learn/blob/master/png/1575118289(1).jpg)



