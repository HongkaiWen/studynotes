读书笔记 - 《大型分布式网站架构设计与实践》

# 集群监控


## 监控指标

**LOAD**

定义:  特定时间间隔内运行队列中的平均数，       一个线程如果满足下面三个条件，就会处于运行队列中。
 * 没有处于IO等待状态
 * 没有主动进入等待状态（wait）
 * 没有被终止。

举例说明：8核cpu 运行16根线程，如果线程平均分配，每个cpu运行队列中有两个线程在运行，如果此状态持续一分钟，那么这一分钟内系统的load值就是2.
 
判断条件：如果load不大于3，系统负载正常；大于5则负载过高。
 
查看方法：uptime\top\dstat

![](/images/monitor/load-uptime.jpg)

![](/images/monitor/load-top.jpg)

![](/images/monitor/load-dstat.jpg)


未完待续...



 
 









