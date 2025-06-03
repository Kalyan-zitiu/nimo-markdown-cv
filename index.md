---
layout: cv
title: Kalyan's Resume
email:
  url: mailto:kalyan.zitiu@gmail.com
  text: kalyan.zitiu@gmail.com
homepage:
  url: https://blog.kalyan.life/
  text: kalyan.life
phone:
  text: 19866803602
city:
 text: Shenzhen, China 
---

<div style="display: flex; justify-content: space-between; align-items: center;">
  <span style="font-size: 50px;"> 黄梓涛</span>
  <img src="https://gcore.jsdelivr.net/gh/Kalyan-zitiu/TyporaIMG/img/tou.jpg" style="width: 200px; height: auto;"/>
</div>


<!--
include contact information from the front matter
Supported arguments:
    - homepage: url, text
    - phone
    - email
-->

{% include cv-contact.html %}
## 教育经历

### 华南理工大学广州学院 本科 计算机学院 软件工程 `2021-至今`

## 工作经验
[**深圳前海道客网络科技有限公司（Daocloud） - 南区交付 - 运维交付**](https://www.daocloud.io/) `2024/7-至今`
+ 负责公司产品的交付生产环境和公司产品的维护保证。
+ 负责自动化运维组件的部署。
+ 处理containerd，kubernetes等容器和容器编排问题。
+ 输出kubernetes生态技术的部署以及使用方案。
+ 处理集群中服务部署的环境问题以及处理兼容性问题。
+ 对重点客户生产环境参与应用运维以及监控维保工作。

[**华南理工大学广州学院 - 机房教学中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021/9-2025/6`

+ 管理语音教学中心的6台linux服务器，保证日常99%时间的平稳运行
+ 深度涉及云服务管理，自动化运维，系统管理，网络管理，服务器管理等。维护多种教学系统的运行。
+ 实现应用程序容器化部署，并使用Kubernetes完成容器部署的编排工作。

[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

+ 熟练掌握并应用Ansible自动化运维工具，实现自动化部署、配置管理及环境监控。
+ 利用Docker和Kubernetes，有效管理和部署容器化应用，提高部署速度、扩展性及系统资源利用率。
+ 实施高级监控解决方案如Prometheus，进行系统和网络性能监控

## 项目经历

### **Contour** **with** **Gateway/Envoy** **云原生网关** **`2025/5-2025/5`**

  通过 **Contour** **作为****控制面**，监听 **Kubernetes 集群**内的HTTPProxy和Ingress资源，下发至 **Envoy** **数据面**。Envoy 作为高性能代理与集群内 **Service 绑定**，支持多域名路由。通过**监控确保数据面健康**。设计网关全链路跟踪，通过**内建收集器**聚合 Span 数据并转发至后端，实现端到端可观测性，保障网关流量可追踪、可诊断。

### **Opentelemetry适配 skywalking java agent深度数据****埋点** **云原生可观测** **`2025/4-2025/5`**

​    主导迁移由skywalking agent **深度****埋点**的业务，进行链路形态转换**为otel 协议**进行收集聚合。保证新链路收集平台对旧数据的兼容，避免大量业务需深入代码层面进行埋点更改。

### **应用skywalking链路监控注入最佳实践 云原生可观测** **`2025/3-2025/4`**

  负责多语言应用在 SkyWalking 中的链路追踪接入以及**多种语言的 Agent 注入**，针对不同的语言应用实现在 Kubernetes 环境下的**自动化和标准化接入流程**。保障追踪数据的一致性与系统稳定性。

### **集群可观测日志中心架构设计以及搭建  云原生可观测** **`2025/2-2025/3`**

  负责日志中心整体架构设计与搭建，解决多系统数据分散与数据孤岛问题，实现**日志、指标和链路追踪**数据的统一采集与集中化管理。通过收集过滤设计，中间件缓存架构，存储等方面解决在可观测**日志、指标和链路追踪**的可靠性，可用性，稳定性。

### **公有云上KafkaCluster日志专线迁移** 云原生可观测** **`2025/1-2025/2`**

  主导针对私有云日志缓冲中间件上云的日志专线迁移。通过VIP以及HAProxy等设计精准对应Kafka broker使用，保证 Kafka 客户端握手时的 `(broker.id ↔ host:port)` 绝对一致，避免元数据错乱、重试风暴和写入失败，同时留下横向扩容的空间。

### **KafKa** **Cluster跨机房集群的数据双向同步** **云原生中间件架构方案** **`2024/12-2025/1`**

 负责 Kafka 集群双向同步方案的设计与落地，针对跨集群数据同步场景，消息打标防环、时间戳冲突处理、分区并行优化等手段，解决了数据一致性、回环问题、性能延迟等核心痛点；同时结合 ACL 同步工具、Checkpoint 机制和监控告警体系，保障了数据零丢失、顺序一致性以及权限同步，成功支持了双活架构、跨地域数据复制及云迁移等高可用场景，提升了系统的稳定性和业务连续性。

### **Redis cluster** **中间件稳定固定IP**  **云原生中间件架构方案** **`2024/10-2025/1`**

  负责保证redis cluster 的直连稳定性，给redis 集群实例附加真实IP，针对pod级别的固定IP模式，避免IP变动的不稳定性导致业务系统断联

### **Rocketmq cluster中间件高可用方案** **云原生中间件架构方案** **`2024/10-2024/11`**

  基于 Kubernetes Operator 部署 RocketMQ 集群，结合 LocalPV 持久化存储保障数据可靠性，针对 Operator 缺陷，重构 Broker 配置规避生产风险。对比多种方案，最终采用 Pod 级静态 IP 绑定，确保 Broker/Namesrv 节点 IP 在集群扩容、故障迁移等场景下永久不变。

### **集群网络方案 云原生集群网络** **`2024/9-2024/10`**

  通过部署 **Cilium** 网络插件并结合 **BGP** **Underlay 模式**，可以实现跨集群的 **Pod 网络互通**和**动态****服务发现**。使得Pod IP及服务类型能被实时通告。集群间的Pod可以**无缝互访debug**，同时动态注册的服务能够被外部网络识别并访问。

### **容器云平台devops/CICD 云原生DevOps工程** **`2024/08-2024/09`**

  基于Jenkins设计并实现CI/CD流水线，启用jenkins 缓存进行流水线加速，集成GitOps与Argo工具链，使用Jenkins Pipeline构建声明式流水线，集成Trivy镜像扫描、优化镜像体积、SonarQube代码质量分析，确保交付安全与质量。除此之外，通过argo 构建多集群应用发布。通过Argo Rollouts实现金丝雀发布与蓝绿部署，结合Prometheus指标自动判断发布状态，支持失败自动回滚，采用GitOps实践，同步Git仓库配置至Kubernete集群，实现基础设施即代码（IaC）。

### **kubernetes集群单机多卡运行Deepseek R1  云原生****大模型****架构****`2025/2-2025/3`**

  在 Kubernetes 集群单机多卡环境下部署 DeepSeek R1 模型的实施工作。该项目采用 Hami 异构和 GPU-Operator，实现高效调度。负责搭建并优化了模型推理环境，利用 DeepSpeed 框架提升了模型的训练效率和推理性能。还设计了自动化部署流程，确保了模型部署的高效性和可扩展性。通过该项目，我们成功实现了大规模语言模型在 Kubernetes 环境下的高效部署和推理，提升了系统的性能和稳定性。

  
## 相关技能
1. **计算机网络**：TCP/IP, HTTP, DNS, WebSocket, RPC
2. **操作系统**：CentOS, Ubuntu, RHEL, Windows,almaLinux
3. **自动化运维工具**：Ansible
4. **可观测技术**：Prometheus,Grafana,Kibana,OpenTelemetry,Victoriametrics,Fluentbit,Jaeger
5. **微服务**：Envoy,Istio,Contour
6. **DevOps**：Jenkins,Argo,Gitops,Argo Rollout,Gitlab
7. **中间件**：Kafka,RocketMQ,Elasticsearch,Redis,MySQL,PostgreSQL,RabbitMQ
8. **容器化**：Containerd,Docker,Podman
9. **容器编排**：Kubernetes
10. **镜像管理**：Harbor,jfrog
11. **集群技术**：Kubean,Kind,MetalLB,Kubespray,Helm,Koordinator
12. **网络技术**：Calico,Cilium
13. **编程技术**：Golang,bash,python

## 个人总结
  对kubernetes生态较为熟悉，容器化技术和容器编排工具经验丰富，熟悉多种集群技术，能够编写自动化脚本，具备网络基础知识，熟悉使用自动化运维工具，掌握不同发行版的Linux系统，掌握基本开发能力。

