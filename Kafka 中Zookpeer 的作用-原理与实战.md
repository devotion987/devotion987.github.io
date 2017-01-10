场景
最近, 运维部门的同事碰到一个问题, 向Kafka 中 某个Topic 发送消息总是失败. 调查下来发现, Zookeeper 中记录的该Topic 的Partition Leader 是一个非法的Broker. 也就是说Zookeeper 中, 记录了错误的Kafka 信息.

重启Kafka 和Zookeeper 后, 该问题得到了解决.

在本篇文章中, 会对Kafka 中Zookeer 的具体作用做一个深入的剖析, 包括理论和实战部分.
