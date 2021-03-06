## 监控

**⚠️注意：该功能为 [Crawlab 专业版](https://www.crawlab.cn/purchase-pro) 专属功能，如需体验此功能，请访问 [演示网站](https://demo.crawlab.cn)。**

对于企业级应用来说，特别是分布式应用服务，经常需要监控各个服务器或数据库的性能指标，例如 CPU、内存、磁盘空间以及网络资源。爬虫管理平台同样不例外，也是需要了解爬虫所在节点的性能状况，以便更合理的分配资源、及时扩容等等。否则，可能会出现一些意料不到的状况。例如，当分布式爬虫抓取的数据量非常大，占满了磁盘空间，这将导致服务器上的应用崩溃；同样的，如果服务器的 CPU 或内存被占满，将导致服务器无法登录、操作或运行应用等问题。这通常都将是灾难性的，如果数据量比较大、应用服务较多，恢复起来也是个很头疼的问题。

为了解决这个问题，我们在 Crawlab 专业版中加入了节点/数据库性能监控功能，以帮助用户更方便的时刻掌握自己分布式节点的性能状况，预测好性能瓶颈，好随时扩容或合理分配资源。

Crawlab 专业版的监控功能主要包括两个：

- 监控概览
- 监控时序图

#### 监控概览

在 Crawlab 专业版首页，我们可以看到 MongoDB 数据库、Redis 数据库、主节点、工作节点的性能数据概览。这些都是及时获取的数据，反应的是当前各个节点数据库的性能状况（如下图）。

![](http://static-docs.crawlab.cn/monitor-home.png)

#### 监控时序图

在 “监控” 页面，我们可以看到各个节点、数据库的性能指标时序图（如下图）。监控时序图能帮助我们了解过去的性能演化情况，通过增长速率预测未来的性能瓶颈，并帮助我们随时采取相应的措施。

![](http://static-docs.crawlab.cn/monitor-time-series.png)

性能指标列表如下：

**节点性能指标**

- 节点 CPU 使用百分比
- 节点总磁盘大小
- 节点磁盘使用量
- 节点磁盘使用百分比
- 节点总内存大小
- 节点内存使用量
- 节点内存使用百分比
- 节点网络接收字节数
- 节点网络发送字节数
- 节点网络接收包数
- 节点网络发送包数

**MongoDB 性能指标**

- MongoDB 平均 Object 大小
- MongoDB Collection 数量
- MongoDB 数据大小
- MongoDB 总文件系统大小
- MongoDB 文件系统使用百分比
- MongoDB 文件系统使用量
- MongoDB 索引大小
- MongoDB 索引数量
- MongoDB 虚拟内存大小
- MongoDB Object 数量
- MongoDB 储存大小

**Redis 性能指标**

- Redis 数据字节数
- Redis Key 数量
- Redis Overhead 总大小
- Redis 峰值分配大小
- Redis 启动分配大小
- Redis 总分配大小