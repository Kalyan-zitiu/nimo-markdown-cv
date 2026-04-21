---
layout: cv
title: Kalyan's Resume
email:
  url: mailto:kalyan.zitiu@gmail.com
  text: kalyan.zitiu@gmail.com
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
# 简历正在修改更新中.....................
## 教育经历
### 华南理工大学广州学院｜本科｜软件工程｜2021.09 - 2025.07
## 在校经历
华南理工大学广州学院｜机房数据中心｜运维组组长｜2021.09 - 2025.06
- 负责校内机房数据中心基础设施与业务系统运维，参与云服务、系统与网络环境管理，保障教学相关业务稳定运行。
- 推动应用容器化改造，并基于 Kubernetes 完成部署编排与运行维护，积累了早期云原生平台实践经验。

## **工作经验**

深圳道客网络科技有限公司（DaoCloud）｜港澳技术团队｜运维开发 / 交付｜2024.07 - 至今

- 面向**7**家客户、累计约 **8** 个项目交付企业级云原生平台，负责 Kubernetes、containerd 及云原生生态组件的部署、升级、兼容性适配与生产问题治理。
- 参与约**40**套集群、累计 **240+** 节点的建设与运维，覆盖日志、监控告警、中间件、数据库、消息队列等基础设施组件，支撑客户业务稳定运行。
- 处理重点客户复杂生产故障与专项问题**32**起，参与架构优化、性能调优和高优先级技术支持，形成容器平台、中间件及基础设施问题闭环能力。
- 参与 AI Infra 场景下 NPU，Metax，Nvidia 等异构算力资源纳管、平台适配与模型服务接入，支撑算力集群落地及对外服务能力建设。
- 在客户现场及交付过程中，沉淀标准化部署、升级、排障与运维流程，提升复杂环境下平台交付效率与稳定性。

## **项目经历**
## **云原生 AI / 大模型基础设施实践**
**技术关键词：Kubernetes / Multi-Cluster / GPU Operator / HAMI / Service Mesh / API Gateway / Cert-Manager / LLM**
#### **概述**
  面向多集群异构算力场景，参与建设 AI Infra 基础设施与模型服务接入能力，覆盖 GPU/NPU 资源纳管、模型服务暴露、安全接入与网络治理等环节。
#### **主要负责内容**
- 面向 **4** 套集群、三类异构算力场景，参与建设 AI Infra 基础设施与模型服务接入能力，覆盖 **Nvidia,Metax,NPU** 等算力资源的统一纳管与平台适配。
- 多集群统一纳管方案落地,支撑3套算力集群接入与资源管理,提升异构环境下的统一运维与交付效率。
- 主导设计vGPU 使用方案,统筹原生开源组件Ascend-mindxl,GPU Operator,HAMI等组件规范集群的GPU管理,适配与问题排查,支撑共享能力,如**sGPU,vNPU资源调度等能力**落地,提升资源使用灵活性与利用率。
- 设计并落地统一模型服务接入方案,对外暴露 30+ 个模型服务,提供标准化接口能力,并结合网关实现基于鉴权方式的访问控制与服务隔离。
- 基于Cert-Manager建设模型服务 TLS 证书签发与生命周期管理能力,支撑**10**个对外服务的安全接入,完善模型服务暴露链路。
- 结合 Service Mesh,Gateway API 或网络策略实现**东西南北的流量治理与访问控制**,提升模型服务安全性与可控性。
- 处理并推动解决兼容性,适配类关键问题,包括典型问题，**如vLLM 适配,NPU 驱动兼容,GPU 共享调度,推理链路接入,证书与网关联调**。

## **云原生可观测体系建设（Tracing / Logging / Metrics）**
**技术关键词：Kubernetes / OpenTelemetry / SkyWalking / Fluent Bit / Vector / Kafka / Elasticsearch / Kibana / Envoy**
#### **概述**
面向云原生多集群场景，建设统一可观测平台，打通日志、指标与链路追踪能力，提升系统观测、故障定位与平台治理能力。
#### **主要负责内容**
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
## **云原生网关与服务治理（Gateway / Envoy）**
**技术关键词：Contour / Envoy / HTTPProxy / Ingress / OpenTelemetry / Kubernetes**
#### **概述**
基于 Contour + Envoy 构建云原生网关体系，支撑集群内统一流量接入、路由转发及网关侧可观测能力建设。
#### **主要负责内容**
+ 基于 Contour 构建网关控制面，监听 Kubernetes 集群内 HTTPProxy、Ingress 等资源，并动态下发至 Envoy 数据面。
+ 基于 Envoy 实现高性能网关流量转发能力，完成与集群内 Service 的联动，支持多域名及复杂路由策略配置。
+ 参与云原生网关接入方案设计与落地，提升集群入口流量管理的标准化与可扩展性。
+ 设计并实施网关数据面健康监控方案，保障流量转发链路的稳定性与可用性。
+ 打通 Envoy 到 OpenTelemetry 及后端观测系统的链路数据采集，增强网关流量的可追踪性与问题定位能力。
#### **项目价值：**
- 建立统一、可扩展、可观测的云原生网关能力，提升集群流量治理水平。
- 为后续 Gateway API 演进及服务治理能力建设奠定基础。
## **云原生网络架构与多集群互通**
**技术关键词：Cilium / eBPF / BGP / Underlay Network / Kubernetes**
#### **概述**
基于 Cilium BGP Underlay 模式设计并落地多集群网络方案，实现跨集群 Pod/Service 网络互通及底层网络可达能力。
#### **主要负责内容**
+ 在 Kubernetes 集群中部署 Cilium 网络插件，基于 BGP Underlay 模式构建云原生网络架构。
+ 实现跨集群 Pod 网络直连互通，打通集群边界，提升多集群场景下的网络连通性。
+ 支持 Pod IP 与 Service IP 向底层网络动态通告，实现云原生网络与物理网络的互联互通。
+ 实现跨集群 Pod 无 NAT 访问与直接调试能力，降低网络路径复杂度并提升问题排查效率。
+ 支撑服务的动态注册与对外访问能力，增强多集群网络架构的可扩展性与可用性。
#### **项目价值：**
- 提升多集群环境下的网络可达性、调试效率与运维便利性。
- 为多活、多地域场景下的云原生架构建设提供网络基础能力。
## **云原生 DevOps 与持续交付体系构建** 
**技术关键词：Jenkins / Argo CD / GitOps / Argo Rollouts / Prometheus / Trivy / SonarQube / Kubernetes**
#### **概述**
围绕容器云平台建设 CI/CD 与 GitOps 持续交付体系，提升多集群环境下的应用交付效率、发布安全性与变更可控性。
#### **主要负责内容**
+ 基于 Jenkins Pipeline 设计并实现声明式 CI/CD 流水线，支撑应用构建、测试与发布流程标准化。
+ 引入构建缓存机制，优化流水线执行效率，缩短应用交付周期。
+ 集成 Trivy 镜像扫描与 SonarQube 代码质量分析，推动安全与质量能力前置。
+ 基于 Argo CD 实现多集群应用持续交付，提升发布过程的一致性与可追溯性。
+ 使用 Argo Rollouts 支持金丝雀发布与蓝绿部署，增强发布灵活性与风险控制能力。
+ 结合 Prometheus 指标实现发布状态自动判断与失败自动回滚，提升发布稳定性。
+ 落地 GitOps 实践，推动应用与基础设施配置的版本化管理与标准化交付。
#### **项目价值：**
- 提升应用交付效率与发布安全性，降低人工操作风险。
- 建立标准化、可观测、可回滚的多集群持续交付体系。
## **相关技能**
+ 云原生与容器编排： Kubernetes、Helm、Kubean、Kubespray、Kind、Koordinator、MetalLB
+ 容器与运行时： Docker、Containerd、Podman
+ AI Infra / 模型服务： vLLM、GPU Operator、HAMI、NVIDIA GPU、MetaX GPU、Ascend NPU、OpenAI-Compatible API
+ 推理优化： KV Cache、Continuous Batching、Tensor Parallelism
+ 自动化与脚本： Ansible、Bash、Python
+ 可观测性： Prometheus、Grafana、Kibana、OpenTelemetry、VictoriaMetrics、Fluent Bit、Vector、Jaeger、SkyWalking
+ 服务治理： Envoy、Istio、Contour、Service Mesh、API Gateway、Cert-Manager
+ DevOps： Jenkins、Argo CD、GitOps、Argo Rollouts、GitLab
+ 中间件： Kafka、RocketMQ、Elasticsearch、Redis、MySQL、PostgreSQL、RabbitMQ
+ 网络： TCP/IP、HTTP、DNS、WebSocket、RPC、Calico、Cilium、BGP
+ 操作系统： CentOS、Ubuntu、RHEL、AlmaLinux、Windows
## **个人总结**
  熟悉 Kubernetes 生态与云原生基础设施，具备容器平台部署、运维、故障排查及自动化运维能力。熟悉多集群管理、可观测性、服务治理、持续交付及常见中间件组件，并具备基于 vLLM、GPU Operator、HAMI 等技术的大模型服务与异构 GPU/NPU 资源管理实践经验，能够支撑云原生平台与 AI 场景下的建设、交付与运维保障工作。
