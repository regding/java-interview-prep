# Java 后端资深工程师 / 架构师面试复习宝典

> 定位：面向 **10+ 年 Java 后端经验** 的资深工程师与架构师候选人。
> 覆盖：Java 语言核心 → JVM → 并发 → 集合源码 → MySQL → Redis → ES → MQ 全家桶 → ZK/Nginx/Netty/Dubbo → Spring 生态 → 分布式与高并发 → 系统设计 → 云原生与大数据 → 工程实践 → 软实力 → 真题速查 → 资源整合。
> 每一章都包含：**核心原理（讲透） + 高频面试题（题干 + 详细解答 + 面试官追问） + 源码分析要点 + 工程实践与踩坑 + 考点速查表**。

---

## 一、这份材料怎么用

| 模式 | 用法 | 适合阶段 |
|---|---|---|
| 系统复习 | 按章节顺序通读，每章先看 TL;DR，再精读原理，最后自测面试题（遮住答案） | 面试前 2~4 周 |
| 查漏补缺 | 用每章末尾「考点速查表」扫一遍，标出不会的考点，只精读对应章节 | 面试前 1 周 |
| 临阵突击 | 只看 25-真题速查 + 各章速查表 + 系统设计案例的「答题框架」 | 面试前 1~2 天 |

## 二、完整目录

### 第一部分 Java 语言与 JVM
| 文件 | 内容 |
|---|---|
| [01-java-core.md](01-java-core.md) | 泛型/反射/代理/IO-NIO/序列化/Java 8~25 新特性全景 |
| [02-jvm.md](02-jvm.md) | 内存结构/类加载/GC 算法与 G1-ZGC/故障排查实战/调优方法论 |
| [03-concurrency.md](03-concurrency.md) | JMM/synchronized 锁升级/AQS 源码/并发容器/线程池源码/虚拟线程 |
| [04-collections-src.md](04-collections-src.md) | HashMap 1.7↔1.8/ConcurrentHashMap/红黑树/LRU/阻塞队列 源码深度 |

### 第二部分 数据库
| 文件 | 内容 |
|---|---|
| [05-mysql.md](05-mysql.md) | 执行流程/InnoDB/索引/MVCC/锁/日志/主从高可用/分库分表/SQL 调优 |
| [06-redis.md](06-redis.md) | 底层数据结构源码/单线程模型/持久化/哨兵集群/缓存三大问题/分布式锁 |
| [07-elasticsearch.md](07-elasticsearch.md) | 倒排索引/写入查询流程/集群脑裂/调优/与 MySQL 同步 |

### 第三部分 消息与中间件
| 文件 | 内容 |
|---|---|
| [08-kafka.md](08-kafka.md) | 存储设计/ISR-HW/幂等事务/消费组 rebalance/可靠性治理 |
| [09-rocketmq-rabbitmq.md](09-rocketmq-rabbitmq.md) | RocketMQ 事务消息/顺序延迟消息/RabbitMQ 原理/MQ 选型对比 |
| [10-zookeeper.md](10-zookeeper.md) | ZAB 协议/选举/Watch/分布式锁/与 etcd 对比 |
| [11-netty.md](11-netty.md) | IO 模型/Reactor/线程模型/零拷贝/粘包拆包/内存池/手写 RPC |
| [12-dubbo-nginx.md](12-dubbo-nginx.md) | Dubbo SPI 源码/负载均衡/集群容错；Nginx 架构/限流/高可用 |

### 第四部分 Spring 生态
| 文件 | 内容 |
|---|---|
| [13-spring-core.md](13-spring-core.md) | IoC 源码/Bean 生命周期/循环依赖三级缓存/AOP/事务传播与失效 |
| [14-spring-boot.md](14-spring-boot.md) | 自动装配源码/启动流程/Starter/配置中心/优雅停机/Spring Boot 3 |
| [15-spring-cloud-mybatis.md](15-spring-cloud-mybatis.md) | 注册中心/网关/OpenFeign/Sentinel/Seata；MyBatis 动态代理与缓存 |

### 第五部分 分布式与高并发
| 文件 | 内容 |
|---|---|
| [16-distributed-basics.md](16-distributed-basics.md) | CAP-BASE/一致性模型/Raft/分布式事务全家桶/分布式锁/分布式 ID/幂等 |
| [17-high-concurrency.md](17-high-concurrency.md) | 缓存一致性/异步化/削峰/限流/熔断降级/隔离/扩容/压测 |
| [18-system-design-methodology.md](18-system-design-methodology.md) | 容量预估/SLA 高可用/架构演进/DDD 微服务拆分/技术选型方法论 |

### 第六部分 系统设计实战
| 文件 | 内容 |
|---|---|
| [19-system-design-cases-1.md](19-system-design-cases-1.md) | 秒杀/短链/抢红包/分布式定时任务/延时任务 |
| [20-system-design-cases-2.md](20-system-design-cases-2.md) | 订单库存/支付对账/IM/Feed 流/搜索/日志监控系统 |
| [21-cloud-native-bigdata.md](21-cloud-native-bigdata.md) | Docker/K8s/Service Mesh/Spark-Flink/Java+AI(LangChain4j) |

### 第七部分 工程实践与软实力
| 文件 | 内容 |
|---|---|
| [22-engineering-practice.md](22-engineering-practice.md) | 设计模式/代码质量/测试/CI-CD/监控四金指标/线上故障排查全流程 |
| [23-algorithms.md](23-algorithms.md) | 高频算法/手写 LRU/海量数据 TopK-去重/布隆过滤器 |
| [24-senior-architect-skills.md](24-senior-architect-skills.md) | 项目答辩/技术选型/带团队/晋升答辩/面试官视角/简历包装 |

### 第八部分 速查与资源
| 文件 | 内容 |
|---|---|
| [25-interview-question-bank.md](25-interview-question-bank.md) | 高频真题速查（阿里/腾讯/字节/美团/京东/拼多多/快手/滴滴/华为） |
| [26-github-repos-books.md](26-github-repos-books.md) | 优质 GitHub 仓库（含用户 star 整合）+ 经典书单 + 学习路线图 |

## 三、学习路线图（资深向）

```
阶段一 地基（约 30% 面试占比）
  01 Java 核心 → 02 JVM → 03 并发 → 04 集合源码
  ⬇ 自测：手写 HashMap 扩容流程 / AQS acquire 流程 / G1 混合回收流程

阶段二 存储（约 30%）
  05 MySQL → 06 Redis → 07 ES
  ⬇ 自测：一条 update SQL 在 InnoDB 的完整旅程 / Redis 主从同步与集群选举

阶段三 中间件与框架（约 25%）
  08 Kafka → 09 RocketMQ → 10 ZK → 11 Netty → 12 Dubbo+Nginx
  13 Spring Core → 14 Boot → 15 Cloud+MyBatis
  ⬇ 自测：说出 Spring 循环依赖三级缓存每级用途 / Kafka ISR 收缩与恢复

阶段四 架构能力（约 15%，但决定定级）
  16 分布式 → 17 高并发 → 18 方法论 → 19/20 系统设计案例
  ⬇ 自测：45 分钟闭卷画秒杀系统架构图 + 容量预估

阶段五 综合
  21 云原生 → 22 工程实践 → 23 算法 → 24 软实力 → 25 真题 → 26 资源
```

## 四、资深/架构师面试的核心策略

1. **原理要能画出来**：任何考点都要能徒手画图讲 5 分钟（HashMap resize、AQS、G1、主从复制、Kafka ISR、Spring 循环依赖）。
2. **每个技术点带一个真实案例**：面试官问「你做过什么」>「你懂什么」。准备 3~5 个带数字的项目故事（STAR 结构）。
3. **源码不是背行号**：讲清「设计动机 → 关键流程 → 取舍 → 如果你来改会怎么改」。
4. **系统设计有框架**：需求澄清 → 容量预估 → 架构图 → 核心流程 → 高可用 → 扩展性 → 风险与取舍，缺一不可（见 18 章方法论）。
5. **主动暴露深度**：资深面试官更怕「什么都答得浅」，宁可少答两个题，也要把一个题挖到源码和权衡层面。

## 五、生产状态（2026-08-14）

| 文件 | 行数 | mermaid 图 | 状态 |
|---|---|---|---|
| [01-java-core.md](01-java-core.md) | 505 | 3 | ✅ |
| [02-jvm.md](02-jvm.md) | 514 | 4 | ✅ |
| [03-concurrency.md](03-concurrency.md) | 588 | 4 | ✅ |
| [04-collections-src.md](04-collections-src.md) | 559 | 4 | ✅ |
| [05-mysql.md](05-mysql.md) | 589 | 4 | ✅ |
| [06-redis.md](06-redis.md) | 571 | 5 | ✅ |
| [07-elasticsearch.md](07-elasticsearch.md) | 527 | 4 | ✅ |
| [08-kafka.md](08-kafka.md) | 537 | 4 | ✅ |
| [09-rocketmq-rabbitmq.md](09-rocketmq-rabbitmq.md) | 521 | 4 | ✅ |
| [10-zookeeper.md](10-zookeeper.md) | 510 | 5 | ✅ |
| [11-netty.md](11-netty.md) | 479 | 5 | ✅ |
| [12-dubbo-nginx.md](12-dubbo-nginx.md) | 475 | 4 | ✅ |
| [13-spring-core.md](13-spring-core.md) | 552 | 4 | ✅ |
| [14-spring-boot.md](14-spring-boot.md) | 525 | 4 | ✅ |
| [15-spring-cloud-mybatis.md](15-spring-cloud-mybatis.md) | 596 | 5 | ✅ |
| [16-distributed-basics.md](16-distributed-basics.md) | 618 | 6 | ✅ |
| [17-high-concurrency.md](17-high-concurrency.md) | 550 | 5 | ✅ |
| [18-system-design-methodology.md](18-system-design-methodology.md) | 540 | 5 | ✅ |
| [19-system-design-cases-1.md](19-system-design-cases-1.md) | 582 | 7 | ✅ |
| [20-system-design-cases-2.md](20-system-design-cases-2.md) | 609 | 9 | ✅ |
| [21-cloud-native-bigdata.md](21-cloud-native-bigdata.md) | 469 | 4 | ✅ |
| [22-engineering-practice.md](22-engineering-practice.md) | 468 | 4 | ✅ |
| [23-algorithms.md](23-algorithms.md) | 592 | 4 | ✅ |
| [24-senior-architect-skills.md](24-senior-architect-skills.md) | 459 | 3 | ✅ |
| [25-interview-question-bank.md](25-interview-question-bank.md) | 451 | 4 | ✅ |
| [26-github-repos-books.md](26-github-repos-books.md) | 175 | 0 | ✅ |

**合计**：26 章 + 总览，共 **13,700+ 行**；全库 **114 张 mermaid 流程图/时序图/状态机图**；**500+ 道面试题**（含详细解答与追问）。另有[「合并版-全部章节.md」](合并版-全部章节.md) 单文件版，方便连续阅读或转存。
