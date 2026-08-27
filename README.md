# Java 后端资深工程师 / 架构师面试复习宝典

> 定位：**双轨制**。主轨面向 **10+ 年 Java 后端经验** 的资深工程师与架构师候选人；辅轨为初学者与转系开发者提供入口（[00 章](00-prerequisite.md) 前置知识 + 双轨学习路线）。
> 覆盖：Java 语言核心 → JVM → 并发 → 集合源码 → MySQL → Redis → ES → MQ 全家桶 → ZK/Nginx/Netty/Dubbo → Spring 生态 → 分布式与高并发 → 系统设计 → 云原生与大数据 → 工程实践 → 软实力 → 真题速查 → 资源整合。
> 每一章都包含：**核心原理（讲透） + 高频面试题（题干 + 详细解答 + 面试官追问） + 源码分析要点 + 工程实践与踩坑 + 考点速查表**。

---

## 一、这份材料怎么用

> 🧭 **你是初学者或从其他语言转来？** 请先读 [00 章 · 前置知识快速总结](00-prerequisite.md)：里面有读者画像自测、Java 世界地图、十个最小前置概念、工具链上手指南与差距自查表，然后按下方「学习路线图」的**初学者轨**走。下表的用法主要面向资深轨读者。

| 模式 | 用法 | 适合阶段 |
|---|---|---|
| 系统复习 | 按章节顺序通读，每章先看「本章速览」，再精读原理，最后自测面试题（遮住答案） | 面试前 2~4 周 |
| 查漏补缺 | 用每章末尾「考点速查表」扫一遍，标出不会的考点，只精读对应章节 | 面试前 1 周 |
| 临阵突击 | 只看 25-真题速查 + 各章速查表 + 系统设计案例的「答题框架」 | 面试前 1~2 天 |

## 二、完整目录

### 第零部分 前置知识（初学者入口）
| 文件 | 内容 |
|---|---|
| [00-prerequisite.md](00-prerequisite.md) | 读者画像与路线 / Java 世界地图 / 十个最小前置概念 / 工具链上手 / 差距自查 30 问 / 五个动手实验 / 非 Java 系迁移对照 |

### 第一部分 Java 语言与 JVM
| 文件 | 内容 | 难度 | 前置 |
|---|---|---|---|
| [01-java-core.md](01-java-core.md) | 泛型/反射/代理/IO-NIO/序列化/Java 8~25 新特性全景 | ●●● | 00 |
| [02-jvm.md](02-jvm.md) | 内存结构/类加载/GC 算法与 G1-ZGC/故障排查实战/调优方法论 | ●●●● | 01 |
| [03-concurrency.md](03-concurrency.md) | JMM/synchronized 锁升级/AQS 源码/并发容器/线程池源码/虚拟线程 | ●●●●● | 02 |
| [04-collections-src.md](04-collections-src.md) | HashMap 1.7↔1.8/ConcurrentHashMap/红黑树/LRU/阻塞队列 源码深度 | ●●●● | 01、03 |

### 第二部分 数据库
| 文件 | 内容 | 难度 | 前置 |
|---|---|---|---|
| [05-mysql.md](05-mysql.md) | 执行流程/InnoDB/索引/MVCC/锁/日志/主从高可用/分库分表/SQL 调优 | ●●●● | 会写 SQL |
| [06-redis.md](06-redis.md) | 底层数据结构源码/单线程模型/持久化/哨兵集群/缓存三大问题/分布式锁 | ●●●● | 00 §2.9 |
| [07-elasticsearch.md](07-elasticsearch.md) | 倒排索引/写入查询流程/集群脑裂/调优/与 MySQL 同步 | ●●● | 05、06 |

### 第三部分 消息与中间件
| 文件 | 内容 | 难度 | 前置 |
|---|---|---|---|
| [08-kafka.md](08-kafka.md) | 存储设计/ISR-HW/幂等事务/消费组 rebalance/可靠性治理 | ●●●● | 16 §2 更佳 |
| [09-rocketmq-rabbitmq.md](09-rocketmq-rabbitmq.md) | RocketMQ 事务消息/顺序延迟消息/RabbitMQ 原理/MQ 选型对比 | ●●●● | 08 |
| [10-zookeeper.md](10-zookeeper.md) | ZAB 协议/选举/Watch/分布式锁/与 etcd 对比 | ●●●● | 16 Raft 节 |
| [11-netty.md](11-netty.md) | IO 模型/Reactor/线程模型/零拷贝/粘包拆包/内存池/手写 RPC | ●●●●● | 01 §5、03 |
| [12-dubbo-nginx.md](12-dubbo-nginx.md) | Dubbo SPI 源码/负载均衡/集群容错；Nginx 架构/限流/高可用 | ●●● | 11、13 |

### 第四部分 Spring 生态
| 文件 | 内容 | 难度 | 前置 |
|---|---|---|---|
| [13-spring-core.md](13-spring-core.md) | IoC 源码/Bean 生命周期/循环依赖三级缓存/AOP/事务传播与失效 | ●●●● | 01 反射/代理 |
| [14-spring-boot.md](14-spring-boot.md) | 自动装配源码/启动流程/Starter/配置中心/优雅停机/Spring Boot 3 | ●●● | 13、会用 Maven |
| [15-spring-cloud-mybatis.md](15-spring-cloud-mybatis.md) | 注册中心/网关/OpenFeign/Sentinel/Seata；MyBatis 动态代理与缓存 | ●●●● | 14、16 CAP 节 |

### 第五部分 分布式与高并发
| 文件 | 内容 | 难度 | 前置 |
|---|---|---|---|
| [16-distributed-basics.md](16-distributed-basics.md) | CAP-BASE/一致性模型/Raft/分布式事务全家桶/分布式锁/分布式 ID/幂等 | ●●●●● | 无硬性，建议先读 10 |
| [17-high-concurrency.md](17-high-concurrency.md) | 缓存一致性/异步化/削峰/限流/熔断降级/隔离/扩容/压测 | ●●●● | 06、16 |
| [18-system-design-methodology.md](18-system-design-methodology.md) | 容量预估/SLA 高可用/架构演进/DDD 微服务拆分/技术选型方法论 | ●●● | 16/17 更佳 |

### 第六部分 系统设计实战
| 文件 | 内容 | 难度 | 前置 |
|---|---|---|---|
| [19-system-design-cases-1.md](19-system-design-cases-1.md) | 秒杀/短链/抢红包/分布式定时任务/延时任务 | ●●●●● | 18 |
| [20-system-design-cases-2.md](20-system-design-cases-2.md) | 订单库存/支付对账/IM/Feed 流/搜索/日志监控系统 | ●●●●● | 18、19 |
| [21-cloud-native-bigdata.md](21-cloud-native-bigdata.md) | Docker/K8s/Service Mesh/Spark-Flink/Java+AI(LangChain4j) | ●●● | 22 更佳 |

### 第七部分 工程实践与软实力
| 文件 | 内容 | 难度 | 前置 |
|---|---|---|---|
| [22-engineering-practice.md](22-engineering-practice.md) | 设计模式/代码质量/测试/CI-CD/监控四金指标/线上故障排查全流程 | ●●●● | 02、13 |
| [23-algorithms.md](23-algorithms.md) | 高频算法/手写 LRU/海量数据 TopK-去重/布隆过滤器 | ●●●● | 语言基础即可 |
| [24-senior-architect-skills.md](24-senior-architect-skills.md) | 项目答辩/技术选型/带团队/晋升答辩/面试官视角/简历包装 | ●● | 有 3+ 年项目经验 |

### 第八部分 速查与资源
| 文件 | 内容 | 难度 | 前置 |
|---|---|---|---|
| [25-interview-question-bank.md](25-interview-question-bank.md) | 高频真题速查（阿里/腾讯/字节/美团/京东/拼多多/快手/滴滴/华为）｜题目带「初级 ✓ / 资深 ★」分层标注 | ●●~●●●● | 对应章节 |
| [26-github-repos-books.md](26-github-repos-books.md) | 优质 GitHub 仓库（精选）+ 经典书单 + 学习路线图 + 三本入门排序 | ● | 无 |

### 第九部分 架构进阶
| 文件 | 内容 | 难度 | 前置 |
|---|---|---|---|
| [27-event-driven-cqrs.md](27-event-driven-cqrs.md) | 事件驱动架构/Event Sourcing/CQRS/Saga/Outbox/CDC | ●●●● | 08/09、16 |
| [28-architecture-patterns.md](28-architecture-patterns.md) | 微服务架构模式全景/中台/Serverless/ADR 决策框架/技术债管理 | ●●● | 15/18 |
| [29-observability-sre.md](29-observability-sre.md) | OpenTelemetry/分布式追踪/日志架构/SLO-SLI/混沌工程/Postmortem | ●●● | 22 监控节 |
| [30-data-api-design.md](30-data-api-design.md) | 数据分层架构/湖仓一体/CDC/RESTful 深度/gRPC/GraphQL/API 治理 | ●●● | 05/12 |
| [31-ai-system-architecture.md](31-ai-system-architecture.md) | LLM 推理架构/RAG 全链路/Agent 架构模式/Java AI 生态/AI 系统陷阱 | ●●● | 21 AI 节更佳 |
| [32-emerging-trends.md](32-emerging-trends.md) | 虚拟线程生产实践/AI 编码协同/可观测性新趋势/Java+AI·MCP/Java 25 LTS 热点 | ●●● | 03 §9、29 |
| [33-jvm-production-troubleshooting.md](33-jvm-production-troubleshooting.md) | JVM 生产排查方法论/OOM全场景/内存泄漏/热点排查/堆外容器/案例集/参数速查 | ●●●●● | 02 |

## 三、学习路线图

### 🧭 初学者轨（从零到能进正文）

```text
第 0 步 前置与自查（约 1~2 周）
  00 前置知识 → 跑通 §3 工具链 → §4 自查表定位自己 → §5 至少做实验 1/2/4
  ⬇ 出口自测：能解释「javac 与 java 的区别」「为什么 counter++ 会丢更新」

第 1 步 语言底子 + 第一个项目（约 1~2 月）
  01 Java 核心(先读用法学) → 14 Spring Boot(做出一个 CRUD Web 项目) → 05 MySQL(会建索引)
  ⬇ 出口自测：独立完成「建表→接口→单测→打包运行」，见 00 章 L4 自查

第 2 步 回头补原理（约 2~3 月）
  04 集合源码 → 02 JVM → 03 并发 → 13 Spring Core → 06 Redis
  ⬇ 出口自测：HashMap 扩容流程 / GC 日志看得懂 / 能说清 @Transactional 失效场景

第 3 步 中间件与架构视野（按需渐进）
  08 Kafka → 16 分布式 → 17 高并发 → 18 方法论 → 19/20 系统设计案例
  ⬇ 出口自测：MQ 消息不丢不重怎么保证 / 45 分钟画秒杀架构

之后：进入下方资深轨，从阶段四开始对齐面试要求。
```

### 🚀 资深轨（10+ 年经验复习向）

```text
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

阶段六 架构进阶（决定架构师定级）
  27 事件驱动+CQRS → 28 架构模式 → 29 可观测性/SRE → 30 数据架构+API → 31 AI 系统架构 → 32 新兴热点
  ⬇ 自测：画 CQRS+Event Sourcing 全链路架构图 / 设计一个 RAG 系统并说明向量库选型理由 / 讲清虚拟线程生产迁移步骤与 Java 25 版本体感

阶段七 JVM 生产排查（高工/架构师必备）
  33 JVM 生产排查实战（含02章深入复习）
  ⬇ 自测：线上 OOM 完整排查流程 / CPU 100% 四步法定位 / 内存泄漏 vs 容量问题判断
```

## 四、资深/架构师面试的核心策略

> 初学者现在不需要读这一节——先把 00 章的自查表通关。等你开始准备真实面试时再回来，它会值回票价。

1. **原理要能画出来**：任何考点都要能徒手画图讲 5 分钟（HashMap resize、AQS、G1、主从复制、Kafka ISR、Spring 循环依赖）。
2. **每个技术点带一个真实案例**：面试官问「你做过什么」>「你懂什么」。准备 3~5 个带数字的项目故事（STAR 结构）。
3. **源码不是背行号**：讲清「设计动机 → 关键流程 → 取舍 → 如果你来改会怎么改」。
4. **系统设计有框架**：需求澄清 → 容量预估 → 架构图 → 核心流程 → 高可用 → 扩展性 → 风险与取舍，缺一不可（见 18 章方法论）。
5. **主动暴露深度**：资深面试官更怕「什么都答得浅」，宁可少答两个题，也要把一个题挖到源码和权衡层面。

## 五、生产状态（2026-08-25）

| 文件 | 行数 | mermaid 图 | 状态 |
|---|---|---|---|
| [00-prerequisite.md](00-prerequisite.md) | 444 | 1 | ✅ 初学者入口 |
| [01-java-core.md](01-java-core.md) | 530 | 3 | ✅ |
| [02-jvm.md](02-jvm.md) | 557 | 4 | ✅ |
| [03-concurrency.md](03-concurrency.md) | 612 | 4 | ✅ |
| [04-collections-src.md](04-collections-src.md) | 577 | 4 | ✅ |
| [05-mysql.md](05-mysql.md) | 610 | 4 | ✅ |
| [06-redis.md](06-redis.md) | 594 | 5 | ✅ |
| [07-elasticsearch.md](07-elasticsearch.md) | 545 | 4 | ✅ |
| [08-kafka.md](08-kafka.md) | 556 | 4 | ✅ |
| [09-rocketmq-rabbitmq.md](09-rocketmq-rabbitmq.md) | 539 | 4 | ✅ |
| [10-zookeeper.md](10-zookeeper.md) | 528 | 5 | ✅ |
| [11-netty.md](11-netty.md) | 496 | 5 | ✅ |
| [12-dubbo-nginx.md](12-dubbo-nginx.md) | 496 | 4 | ✅ |
| [13-spring-core.md](13-spring-core.md) | 570 | 4 | ✅ |
| [14-spring-boot.md](14-spring-boot.md) | 542 | 4 | ✅ |
| [15-spring-cloud-mybatis.md](15-spring-cloud-mybatis.md) | 616 | 5 | ✅ |
| [16-distributed-basics.md](16-distributed-basics.md) | 639 | 6 | ✅ |
| [17-high-concurrency.md](17-high-concurrency.md) | 569 | 5 | ✅ |
| [18-system-design-methodology.md](18-system-design-methodology.md) | 561 | 5 | ✅ |
| [19-system-design-cases-1.md](19-system-design-cases-1.md) | 597 | 7 | ✅ |
| [20-system-design-cases-2.md](20-system-design-cases-2.md) | 624 | 9 | ✅ |
| [21-cloud-native-bigdata.md](21-cloud-native-bigdata.md) | 485 | 4 | ✅ |
| [22-engineering-practice.md](22-engineering-practice.md) | 514 | 4 | ✅ |
| [23-algorithms.md](23-algorithms.md) | 607 | 4 | ✅ |
| [24-senior-architect-skills.md](24-senior-architect-skills.md) | 476 | 3 | ✅ |
| [25-interview-question-bank.md](25-interview-question-bank.md) | 508 | 4 | ✅ |
| [26-github-repos-books.md](26-github-repos-books.md) | 198 | 0 | ✅ |
| [27-event-driven-cqrs.md](27-event-driven-cqrs.md) | 478 | 6 | ✅ |
| [28-architecture-patterns.md](28-architecture-patterns.md) | 483 | 5 | ✅ |
| [29-observability-sre.md](29-observability-sre.md) | 466 | 5 | ✅ |
| [30-data-api-design.md](30-data-api-design.md) | 485 | 3 | ✅ |
| [31-ai-system-architecture.md](31-ai-system-architecture.md) | 598 | 8 | ✅ |
| [32-emerging-trends.md](32-emerging-trends.md) | 214 | 0 | ✅ |

**合计**：33 章（含 00 前置知识章）+ 总览，共 **17,314+ 行**（约 17,300 行）；全库 **142 张 mermaid 流程图/时序图/状态机图**；**500+ 道面试题**（含详细解答与追问）。另有[「合并版-全部章节.md」](合并版-全部章节.md) 单文件版，方便连续阅读或转存。
