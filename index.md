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
### 华南理工大学广州学院 本科毕业 计算机学院 软件工程 `2021-2025`
主修计算机网络工程，计算机组成原理，高级算法，AWS云工程，微服务架构开发。

## 在校经历
[**华南理工大学广州学院 - 机房数据中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021/9-2025/6`

+ 负责学院机房数据中心基础设施的建设、运维与日常管理，保障学院业务系统稳定运行。
+ 参与云服务、自动化运维、系统管理、网络管理及服务器管理等相关工作，支撑多类教学系统的部署与维护。
+ 推动应用容器化改造，并基于 Kubernetes 完成容器编排、部署与运行维护。

[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

+ 参与团队相关软件环境的部署与运维，使用 Ansible 实现自动化部署、配置管理及基础环境维护。
+ 使用 Docker 与 Kubernetes 管理和部署容器化应用，提升应用交付效率与系统扩展能力。
+ 基于 Prometheus 搭建监控能力，对系统及网络运行状态进行监控与性能观测。

**## 工作经验**
[**深圳道客网络科技有限公司（Daocloud） - 港澳技术团队 - 运维开发&&交付**](https://www.daocloud.io/) `2024/7-至今`
+ 负责企业级云原生平台在客户生产环境的交付落地、运维保障与问题治理。
+ 承担 Kubernetes、containerd 及云原生生态组件的部署、升级、兼容性适配与故障处置。
+ 参与数据库、消息队列、日志中心、监控告警等中间件与平台基础设施的建设和维护。
+ 面向重点客户生产环境，负责复杂故障排查、架构优化及专项技术支持。
+ 参与 AI Infra 场景下异构 GPU/NPU 资源纳管与平台适配，支撑算力集群落地使用。


## 项目经历

### **云原生 AI / 大模型基础设施实践**

**技术关键词：Kubernetes / Multi-Cluster / GPU Operator / HAMI / Service Mesh / API Gateway / Cert-Manager / LLM**

#### 概述
  基于容器云平台，实现多集群统一管理以及不同类型的算力管理
#### 主要负责内容
+ 负责多集群统一纳管方案设计与落地，支撑不同算力类型集群的统一接入、管理与使用。
+ 面向 NVIDIA、MetaX 及 NPU 等异构算力环境，完成集群部署、资源接入及统一服务化暴露。
+ 基于 GPU Operator 与 HAMI 实现 vGPU 能力管理与调度，提升异构算力资源利用率与分配灵活性。
+ 设计统一模型服务接入方案，对外提供标准化 API，并结合网关实现基于 Key 的权限控制与访问隔离。
+ 基于外部签注机构与 Cert-Manager 实现 TLS 证书统一签发与生命周期管理，完善模型服务安全接入体系。
+ 结合业务要求实施严格网络治理，基于 Service Mesh 对各集群流量进行隔离、管控与服务间访问治理。
+ 参与统一模型部署平台建设，支撑模型的部署、运行、访问与日常使用管理，并验证其稳定性与性能表现。

#### **项目价值：**
- 完成多集群与异构算力资源的统一纳管，为 AI 基础设施平台化建设提供落地实践。
- 验证云原生平台承载大模型服务的可行性，沉淀模型部署、服务暴露与安全治理的实现方案。
- 提升算力资源利用率与模型服务管理效率，为后续统一调度、标准化接入及平台扩展奠定基础。


### **云原生可观测体系建设（Tracing / Logging / Metrics）**

**技术关键词：Kubernetes / OpenTelemetry / SkyWalking / Fluent Bit / Vector / Kafka / Elasticsearch / Kibana / Envoy**

#### 概述
面向云原生多集群场景，建设统一可观测平台，打通日志、指标与链路追踪能力，提升系统观测、故障定位与平台治理能力。
#### 主要负责内容
+ 设计并落地覆盖网关、应用、中间件及 Kubernetes 集群的统一可观测体系，实现日志、指标、链路追踪的集中化管理。
+ 基于 Fluent Bit、Vector、Kafka、Elasticsearch、Kibana 构建日志采集、传输、缓冲、存储与检索链路，提升日志治理能力。
+ 以 OpenTelemetry 作为统一观测协议，兼容 SkyWalking Java Agent 历史链路数据，降低业务改造成本并保障观测连续性。
+ 负责 SkyWalking 向 OpenTelemetry 的链路迁移与数据聚合改造，确保新旧链路数据的一致性与平滑过渡。
+ 负责多语言应用在 Kubernetes 环境下的 Agent 自动化注入与标准化部署方案，提升链路采集一致性与运维效率。
+ 参与 Kafka 日志链路迁移方案落地，保障跨环境迁移过程中链路稳定与数据一致性。

#### **项目价值：**
- 构建统一的云原生可观测底座，支撑多集群及复杂业务场景下的运行观测与治理。
- 在降低业务侧改造成本的前提下完成观测体系升级，保障平台平稳演进。
- 提升日志检索、链路分析与故障定位效率，增强系统可诊断性与运维支撑能力。

### 云原生网关与服务治理（Gateway / Envoy）

**技术关键词：Contour / Envoy / HTTPProxy / Ingress / OpenTelemetry / Kubernetes**

#### 概述
基于 Contour + Envoy 构建云原生网关体系，支撑集群内统一流量接入、路由转发及网关侧可观测能力建设。
#### 主要负责内容
+ 基于 Contour 构建网关控制面，监听 Kubernetes 集群内 HTTPProxy、Ingress 等资源，并动态下发至 Envoy 数据面。
+ 基于 Envoy 实现高性能网关流量转发能力，完成与集群内 Service 的联动，支持多域名及复杂路由策略配置。
+ 参与云原生网关接入方案设计与落地，提升集群入口流量管理的标准化与可扩展性。
+ 设计并实施网关数据面健康监控方案，保障流量转发链路的稳定性与可用性。
+ 打通 Envoy 到 OpenTelemetry 及后端观测系统的链路数据采集，增强网关流量的可追踪性与问题定位能力。

#### **项目价值：**
- 建立统一、可扩展、可观测的云原生网关能力，提升集群流量治理水平。
- 为后续 Gateway API 演进及服务治理能力建设奠定基础。

  
### **云原生网络架构与多集群互通**

**技术关键词：Cilium / eBPF / BGP / Underlay Network / Kubernetes**

#### 概述
基于 Cilium BGP Underlay 模式设计并落地多集群网络方案，实现跨集群 Pod/Service 网络互通及底层网络可达能力。
#### 主要负责内容
+ 在 Kubernetes 集群中部署 Cilium 网络插件，基于 BGP Underlay 模式构建云原生网络架构。
+ 实现跨集群 Pod 网络直连互通，打通集群边界，提升多集群场景下的网络连通性。
+ 支持 Pod IP 与 Service IP 向底层网络动态通告，实现云原生网络与物理网络的互联互通。
+ 实现跨集群 Pod 无 NAT 访问与直接调试能力，降低网络路径复杂度并提升问题排查效率。
+ 支撑服务的动态注册与对外访问能力，增强多集群网络架构的可扩展性与可用性。
  
#### **项目价值：**
- 提升多集群环境下的网络可达性、调试效率与运维便利性。
- 为多活、多地域场景下的云原生架构建设提供网络基础能力。

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

