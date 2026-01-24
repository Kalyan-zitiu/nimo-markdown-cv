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
### 广东省清远市清城区第二中学
### 华南理工大学广州学院 本科 计算机学院 软件工程 `2021-2025`

## 工作经验
[**深圳道客网络科技有限公司（Daocloud） - 南区 - 运维交付**](https://www.daocloud.io/) `2024/7-至今`
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


### **云原生 AI / 大模型基础设施实践**  项目周期：2025/02 – 2025/03

**技术关键词：Kubernetes / GPU Operator / HAMI / DeepSpeed / LLM**

#### **云原生集群的多机多卡以及单机多卡的模型运行效率以及算力优化**
- 在 Kubernetes 单机多 GPU 环境下VLLM落地运行 **DeepSeek R1** 大模型
- 通过 **GPU Operator + HAMI** 实现异构 vGPU能力 的统一管理与高效调度
- 基于 **DeepSpeed** 框架优化模型推理与训练性能
- 设计并实现模型的自动化部署流程，提升部署效率与可扩展性
- 验证大模型在 Kubernetes 环境下运行的稳定性与性能表现
- 通过优化KV Cache提升模型运行性能

#### **项目价值：**
- 验证云原生平台承载大模型推理的可行性
- 为后续 AI 平台与算力调度体系建设提供实践基础
- 提高模型的运行效率以及算力资源使用率


### **云原生可观测体系建设（Tracing / Logging / Metrics）** 项目周期：2025/01 – 2025/05

**技术关键词：OpenTelemetry / SkyWalking / Envoy / Kafka / Kubernetes**

#### **云原生全链路可观测平台建设**
- 设计并落地覆盖 **网关、应用、中间件、集群** 的统一可观测体系，实现 **日志、指标、链路追踪三位一体** 的集中化管理
- 以 **OpenTelemetry** 作为统一观测协议，兼容 **SkyWalking Java Agent 深度埋点** 的历史链路数据，避免业务侧侵入式改造
- 主导 **SkyWalking → OpenTelemetry 协议** 的链路形态迁移与数据聚合改造，确保新旧链路数据连续性与一致性
- 负责多语言应用在 Kubernetes 环境下的 **SkyWalking Agent 自动化、标准化注入方案**，保障链路采集的一致性与系统稳定性
- 设计并搭建集群级日志中心架构，通过 **采集、过滤、缓冲、存储** 分层设计，解决日志分散与数据孤岛问题
- 主导 **Kafka 日志专线迁移（私有云 → 公有云）**，通过 VIP 与 HAProxy 精准映射 Broker，确保 `(broker.id ↔ host:port)` 一致，避免元数据错乱与重试风暴

#### **项目价值：**
- 构建企业级云原生可观测底座，支撑多集群与复杂业务场景
- 在不中断业务的前提下完成观测体系升级
- 显著提升故障定位效率与系统可诊断能力

### 云原生网关与服务治理（Gateway / Envoy） 项目周期：2025/05 ～2025/06

**技术关键词：Contour / Envoy / HTTPProxy / Ingress / OpenTelemetry**

#### **基于 Contour + Envoy 的云原生网关体系**
- 以 **Contour** 作为控制面，监听 Kubernetes 集群内 **HTTPProxy / Ingress** 资源，并动态下发至 **Envoy 数据面**
- 基于 Envoy 构建高性能云原生网关，与集群内 Service 深度绑定，支持多域名与复杂路由策略
- 设计并实施 **网关数据面健康监控方案**，保障流量转发稳定性
- 打通 **Envoy → OpenTelemetry → 后端观测系统** 的全链路追踪能力，实现网关流量端到端可观测
- 通过内建收集器聚合 Span 数据，保障流量可追踪、问题可回溯、异常可诊断

#### **项目价值：**
- 建立可观测、可扩展的云原生网关能力
- 为 Gateway API 与后续服务治理演进奠定基础
现了大规模语言模型在 Kubernetes 环境下的高效部署和推理，提升了系统的性能和稳定性。

### **云原生中间件高可用与跨集群架构** 项目周期：2024/10 – 2025/02

**技术关键词：Kafka / Redis / RocketMQ / Kubernetes Operator / 跨集群同步**

#### **云原生中间件高可用与跨地域架构实践**
- 负责 **Kafka 跨机房双向同步方案** 的整体设计与落地：
- 消息打标防回环
- 时间戳冲突处理
- 分区并行与性能优化
- ACL 同步、Checkpoint 机制与监控告警体系建设
- 成功支撑 **双活架构、跨地域数据复制与云迁移** 场景，保障数据零丢失与顺序一致性
- 针对 **Redis Cluster** 设计 **Pod 级真实 IP / 固定 IP 方案**，避免 IP 漂移导致的业务断联
- 基于 Kubernetes Operator 部署 **RocketMQ 集群**，结合 LocalPV 提供持久化能力
- 针对 Operator 缺陷，重构 Broker 配置以规避生产环境风险
- 采用 Pod 级静态 IP 绑定，确保 Broker / NameSrv 在扩容与故障迁移场景下 IP 永久不变
  
#### **项目价值：**
- 显著提升云原生中间件在生产环境下的稳定性与可运维性
- 为核心业务提供高可用、可扩展的消息与缓存基础设施

### **云原生网络架构与多集群互通** 项目周期：2024/09 – 2024/10

**技术关键词：Cilium / eBPF / BGP / Underlay Network**

#### **基于 Cilium BGP Underlay 的多集群网络方案**
- 在 Kubernetes 集群中部署 **Cilium** 网络插件，采用 **BGP Underlay 模式**
- 实现跨集群 **Pod 网络直连互通**，打破集群边界
- Pod IP 与 Service IP 可动态通告至底层网络，实现真实网络可达
- 支持跨集群 Pod 无 NAT 调试与直接访问
- 实现服务的动态注册与外部网络访问能力
  
#### **项目价值：**
- 提升多集群调试与运维效率
- 为多活、多地域云原生架构提供网络基础能力

### **云原生 DevOps 与持续交付体系构建** 项目周期：2024/08 – 2024/09

**技术关键词：Jenkins / Argo CD / GitOps / Argo Rollouts / Prometheus**

#### **容器云平台 CI/CD 与 GitOps 实践**
- 基于 **Jenkins Pipeline** 设计并实现声明式 CI/CD 流水线
- 引入构建缓存机制，显著提升流水线执行效率
- 集成 **Trivy 镜像扫描** 与 **SonarQube 代码质量分析**，实现安全与质量左移
- 基于 **Argo CD** 实现多集群应用的持续交付
- 使用 **Argo Rollouts** 支持金丝雀发布与蓝绿部署
- 结合 **Prometheus 指标** 自动判断发布状态，支持失败自动回滚
- 落地 GitOps 实践，实现基础设施即代码（IaC）
  
#### **项目价值：**
- 提升应用交付效率与发布安全性
- 建立标准化、可回滚的多集群交付体系

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

