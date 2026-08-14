[📖 返回目录](README.md) · [⬅️ 上一章](25-interview-question-bank.md)

# 26. 优质资源整合：GitHub 仓库（含用户 star 清单）+ 经典书单 + 学习路线

> 本章整合了 **regding 账号 star 的 295 个仓库** 中与 Java 后端/分布式/系统设计/面试直接相关的部分，
> 按「面试复习价值」分类整理；另附经典书单与刷题路线。标注 ⭐ 的为高优先级。

---



### 📑 本章目录

- [一、面试/知识体系类（star 整合）](#一面试知识体系类star-整合)
- [二、Java 语言/JVM/源码类（star 整合）](#二java-语言jvm源码类star-整合)
- [三、数据库/中间件源码类（star 整合）](#三数据库中间件源码类star-整合)
- [四、安全/认证授权类（star 整合）](#四安全认证授权类star-整合)
- [五、云原生/大数据/新趋势类（star 整合）](#五云原生大数据新趋势类star-整合)
- [六、网络/系统底层类（star 整合，进阶选修）](#六网络系统底层类star-整合进阶选修)
- [七、经典书单（按章节配套）](#七经典书单按章节配套)
- [八、刷题与练习路线](#八刷题与练习路线)
- [九、其他已 star 但非主线（一句话归类）](#九其他已-star-但非主线一句话归类)

## 一、面试/知识体系类（star 整合）

| 仓库 | 说明 | 建议用法 |
|---|---|---|
| ⭐ Snailclimb/JavaGuide | Java 面试 & 后端通用面试指南，覆盖计算机基础/数据库/分布式/高并发/系统设计 | 主线复习索引，对照本材料查漏 |
| ⭐ doocs/advanced-java | 互联网 Java 工程师进阶知识：高并发/分布式/中间件深度文章 | 分布式、高并发章节的延伸阅读 |
| ⭐ CyC2018/CS-Notes | 技术面试必备基础知识（OS/网络/数据库/系统设计） | 计算机基础速查 |
| InterviewMap/CS-Interview-Knowledge-Map | 面试知识地图（JS/网络/浏览器为主） | 网络部分补充 |
| wx-chevalier/DistributedSystem-Notes | 深入浅出分布式基础架构（DB/网络/分布式系统/大数据/云） | 分布式理论延伸 |
| huihut/interview | C/C++ 面试总结（含系统/网络/链接装载） | 对比阅读，理解底层 |
| ⭐ donnemartin/system-design-primer | 系统设计面试圣经（英文） | 对照 19/20 章案例练习 |
| InterviewReady/system-design-resources | 系统设计资源合集（英文） | 案例库 |
| ⭐ labuladong/fucking-algorithm | 算法刷题框架（中文，讲套路） | 配合 23 章刷题 |
| soulmachine/algorithm-essentials | 算法精粹，举一反三 | 算法总复习 |
| kevin-wayne/algs4 | 算法第 4 版配套代码 | 基础数据结构补课 |
| julycoding/The-Art-Of-Programming-By-July-2nd | 编程之法：面试和算法心得 | 经典题集 |
| EbookFoundation/free-programming-books | 免费编程书（英文） | 找书 |
| justjavac/free-programming-books-zh_CN | 免费中文编程书 | 找书 |
| jobbole/awesome-programming-books | 经典编程书籍大全 | 书单参考 |
| ossu/computer-science | 自学 CS 路线 | 体系补课 |
| nilbuild/developer-roadmap | 交互式开发者路线图 | 全景图 |
| codecrafters-io/build-your-own-x | 从零实现数据库/Redis/OS 等 | 深度理解中间件原理 |

## 二、Java 语言/JVM/源码类（star 整合）

| 仓库 | 说明 | 建议用法 |
|---|---|---|
| ⭐ openjdk/jdk | JDK 主线源码 | 查源码第一手资料 |
| unofficial-openjdk/openjdk | OpenJDK 各分支镜像 | 同上 |
| ⭐ waylau/java-virtual-machine-specification | 《Java 虚拟机规范（第 11 版）》中文翻译 | 配合 02 章 |
| dougqh/jvm-mechanics | HotSpot 编译与反优化演示 | JIT 深度 |
| eclipse-openj9/openj9 | OpenJ9 JVM | 了解备选 JVM |
| ozy/ToyJVM | C 实现的实验性 JVM 字节码解释器 | 理解 JVM 本质 |
| shudo/shujit | Java JIT 编译器（x86） | JIT 原理 |
| ⭐ CarpenterLee/JCFInternals | 深入理解 Java 集合框架 | 配合 04 章源码 |
| CarpenterLee/JavaLambdaInternals | 深入理解函数式编程与 Streams | 配合 01 章 |
| crossoverJie/JCSprout | Java Core 基础/并发/算法 | 复习补充 |
| google/guava | Google 核心 Java 库 | 工具类/并发补充 |
| classgraph | 超快 classpath 扫描器 | 理解 Spring 扫描原理 |
| google/gson / alibaba/fastjson | JSON 库（fastjson 2.x 推荐） | 序列化对比 |
| x-stream/xstream | Java 对象 XML 序列化 | 序列化对比 |
| byte-buddy / cglib | 运行时字节码生成 | 配合 AOP/代理原理 |
| alibaba/arthas | Java 诊断利器 | 配合 02 章排查实战 |
| btraceio/btrace | 生产环境动态追踪 | 排查进阶 |
| alibaba/jvm-sandbox | 基于 JVM 的非侵入 AOP 容器 | 理解字节码增强 |
| LMAX-Exchange/disruptor | 高性能线程间消息库 | 高并发/无锁进阶 |
| RxJava / vert.x / akka-core | 响应式与 Actor | 响应式编程对比 |
| oracle/graal | GraalVM 原生镜像 | 配合 14 章 Boot3 |

## 三、数据库/中间件源码类（star 整合）

| 仓库 | 说明 | 建议用法 |
|---|---|---|
| ⭐ mysql/mysql-server | MySQL 官方源码 | 05 章源码级延伸 |
| mackyle/sqlite / cstack/db_tutorial | SQLite 源码 / 从零写 SQLite | 理解存储引擎本质 |
| cmu-db/peloton | 自驱动数据库 | 前沿 |
| ⭐ redis/jedis、redis/hiredis | Redis 官方 Java/C 客户端 | 客户端原理 |
| ⭐ redisson/redisson | Redisson：分布式锁/数据结构 | 配合 06 章锁源码 |
| ⭐ antirez/sds | Redis 作者 SDS 字符串库源码 | 配合 06 章 SDS |
| ⭐ elastic/elasticsearch | ES 源码 | 07 章延伸 |
| ⭐ apache/kafka | Kafka 源码 | 08 章延伸 |
| ⭐ apache/rocketmq | RocketMQ 源码 | 09 章延伸 |
| ⭐ apache/zookeeper | ZooKeeper 源码 | 10 章延伸 |
| ⭐ etcd-io/etcd | etcd（Raft 实现） | 10 章对比 |
| ⭐ apache/dubbo | Dubbo RPC 框架源码 | 12 章延伸 |
| ⭐ netty/netty | Netty 源码 | 11 章延伸 |
| ⭐ nginx/nginx | Nginx 源码 | 12 章延伸 |
| ⭐ apache/tomcat | Tomcat 源码 | Web 容器原理 |
| pkpk1234/BeggarServletContainer-doc | 手写 Servlet 容器系列 | 理解 Tomcat 本质 |
| MyCATApache/Mycat-Server | MyCat 分库分表中间件 | 05 章对比 ShardingSphere |
| alibaba/nacos | Nacos：注册中心+配置中心 | 15 章核心 |
| hazelcast/hazelcast | 分布式数据平台 | 分布式缓存备选 |
| grpc/grpc-java / apache/thrift | gRPC/Thrift RPC 框架 | RPC 协议对比 |
| tang-jie/NettyRPC / fengjiachun/Jupiter | 基于 Netty 的 RPC 框架 | 手写 RPC 参考 |
| sofastack/sofa-jarslink | 多应用部署插件（SOFAArk） | 模块化/热部署 |
| lindzh/hasting | Java NIO 分布式跨语言服务框架 | RPC 演进参考 |
| apache/mesos | 分布式资源管理 | 容器调度史 |

## 四、安全/认证授权类（star 整合）

| 仓库 | 说明 | 建议用法 |
|---|---|---|
| ⭐ apache/shiro | Shiro 安全框架 | 配合 15 章认证授权 |
| ⭐ **regding/shiro-redis** | **你的项目**：Shiro 默认只支持 ehcache/ConcurrentHashMap 会话，本项目实现 Redis 支持 | 面试「项目经验」可直接用：分布式会话/权限缓存改造 |
| apereo/cas + java-cas-client | CAS 单点登录 | SSO 原理 |
| scribejava/scribejava | 简单 OAuth 库 | OAuth2 流程 |
| tink-crypto/tink | 多语言密码学库 | 加密方案选型 |
| FeeiCN/Cobra | 源代码安全审计 | 安全工程 |

## 五、云原生/大数据/新趋势类（star 整合）

| 仓库 | 说明 | 建议用法 |
|---|---|---|
| ⭐ kubernetes/kubernetes | K8s 源码 | 21 章核心 |
| docker/compose | Docker Compose | 本地环境编排 |
| wagoodman/dive | 分析 docker 镜像分层 | 镜像优化 |
| 99cloud/training-kubernetes | K8s 训练教程 | 21 章补充 |
| apache/spark | Spark 源码 | 21 章大数据 |
| apache/logging-flume | Flume 日志采集 | 日志系统 |
| ray-project/ray | AI 计算引擎 | 新趋势 |
| ⭐ langchain4j/langchain4j | Java 生态 LLM 应用框架 | 21 章 Java+AI |
| GoogleContainerTools/jib | Java 应用容器化构建 | 工程实践 |
| scala/scala | Scala 2 编译器 | 了解 JVM 语言 |
| gradle/gradle | Gradle 构建 | 构建工具对比 Maven |
| bazelbuild/bazel / facebook/buck | 大型构建系统 | 构建演进 |
| codecentric/spring-boot-admin | Spring Boot 监控 UI | 监控实践 |
| hazelcast / apache/mesos | 见上 | - |

## 六、网络/系统底层类（star 整合，进阶选修）

zhiyong0804/net_io（IO 模型详解）、grpc/grpc-go、antirez/sds、jamesroutley/write-a-hash-table、petewarden/c_hashmap、cstack/db_tutorial、libuv/libuv（异步 I/O）、tinyhttpd（500 行 HTTP Server）、the-super-tiny-compiler（最小编译器）、rui314/9cc（C 编译器）、cfenollosa/os-tutorial（从零写 OS）、LearningOS/rust-based-os-comp2023、qemu/qemu、learn-kvm（你的仓库：QEMU/KVM 学习笔记）、torvalds/linux、git/git、curl/curl、nginx/nginx。

> 这些不是面试主线，但「从零写一个 XX」的仓库是资深面试官最喜欢的深度话题来源，
> 挑 1~2 个精读（如 Tinyhttpd / write-a-hash-table / db_tutorial），面试时能讲「自己读过源码」的底层细节非常加分。

## 七、经典书单（按章节配套）


### JVM 与 Java 语言
- 《深入理解 Java 虚拟机（第 3 版）》周志明 —— 02 章必读，没有之一
- 《Java 虚拟机规范（Java SE 8/11 版）》—— 规范原文
- 《Java 并发编程的艺术》方腾飞 —— 03 章
- 《Java 并发编程实战》Brian Goetz —— 并发圣经
- 《Effective Java（第 3 版）》—— 语言最佳实践

### 数据库
- 《高性能 MySQL（第 3 版）》—— 05 章
- 《MySQL 技术内幕：InnoDB 存储引擎（第 2 版）》姜承尧 —— 05 章引擎细节
- 《Redis 设计与实现》黄健宏 —— 06 章底层数据结构必读
- 《Redis 开发与运维》付磊/张益军 —— 06 章运维实战

### 中间件
- 《深入理解 Kafka：核心设计与实践原理》朱忠华 —— 08 章
- 《RocketMQ 技术内幕》丁威 —— 09 章
- 《Netty 权威指南（第 2 版）》李林锋 —— 11 章
- 《ZooKeeper：分布式过程协同技术详解》—— 10 章

### Spring
- 《Spring 揭秘》计文柯 —— 13 章 IoC/AOP 思路
- 《Spring 源码深度解析》郝佳 —— 13/14 章源码
- 《MyBatis 技术内幕》徐郡明 —— 15 章

### 分布式与架构
- 《数据密集型应用系统设计（DDIA）》Martin Kleppmann —— 16~18 章必读，架构师圣经
- 《凤凰架构》周志明 —— 微服务演进最佳中文读物
- 《分布式系统设计》/ 《大规模分布式存储系统》杨传辉 —— 分布式理论
- 《系统设计面试（第 1/2 辑）》Alex Xu —— 19/20 章案例
- 《架构整洁之道》Robert Martin —— 工程实践
- 《SRE：Google 运维解密》—— 22 章监控/可靠性
- 《重构：改善既有代码的设计》Martin Fowler —— 22 章

### 算法
- 《剑指 Offer》—— 面试题经典
- 《算法（第 4 版）》Sedgewick —— 基础
- 《labuladong 的算法小抄》—— 刷题套路

## 八、刷题与练习路线

1. **算法**：LeetCode 热题 100 + 剑指 Offer，按 23 章的分类刷（链表/树/DP/滑动窗口/海量数据）。
2. **手写源码**：HashMap 简化版、LRU、线程池简化版、AQS 简化版、雪花 ID、布隆过滤器 —— 面试现场手写高频。
3. **系统设计**：每周 1 题，按 18 章框架闭卷画图 + 口述 20 分钟，用 donnemartin/system-design-primer 对答案。
4. **面经**：牛客网 Java 面经 + 25 章真题速查滚动复习。

## 九、其他已 star 但非主线（一句话归类）

- AI/Agent 类（langchain、opencode、superpowers、dify、LangChain4j、happy-llm、R1、JARVIS、alpaca）：AI 工程化趋势，见 21 章「Java + AI」小节，也可作为面试「技术视野」话题。
- 系统/工具类（vim、nvim-config、ohmyzsh、linux、qemu、FFmpeg、vcpkg、git、curl）：工程效率。
- C/C++/编译器/OS 类（9cc、mal、db_tutorial、os-tutorial、linux、torvalds/linux、rust、racket、godot）：底层兴趣，深度话题素材。
- 其他（free-for-dev、howto-make-more-money、programmer-job-blacklist、996.ICU、run 润学）：职业与合规话题，面试「为什么离职」可参考但谨慎使用。
