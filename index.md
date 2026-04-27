---
layout: cv
title: Kalyan's Resume
email:
  url: mailto:kalyan.zitiu@gmail.com
  text: kalyan.zitiu@gmail.com
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
## **教育经历**
### 华南理工大学广州学院｜本科｜软件工程｜2021.09 - 2025.07
#### 校园经历
华南理工大学广州学院｜机房数据中心｜运维组组长｜2021.09 - 2025.06
- 负责校内机房数据中心基础设施与业务系统运维，参与云服务、系统与网络环境管理，保障教学相关业务稳定运行。
- 推动应用容器化改造，并基于 Kubernetes 完成部署编排与运行维护，积累了早期云原生平台实践经验。

## **工作经验**
### **深圳道客网络科技有限公司（DaoCloud）｜粤港澳技术团队｜[运维开发/交付/解决方案]｜2024.07 - 至今**
- 目前个人面向**7**家客户、累计约 **8** 个项目交付企业级云原生平台，负责 Kubernetes、containerd 及云原生生态组件的部署、升级、兼容性适配与生产问题治理。
- 个人参与统筹管理约**40**套集群、累计 **240+** 节点的建设与运维，覆盖日志、监控告警、中间件、数据库、消息队列等基础设施组件，支撑客户业务稳定运行。
- 个人负责处理重点客户复杂生产故障与专项问题**32**起，参与架构优化、性能调优和高优先级技术支持，形成容器平台、中间件及基础设施问题闭环能力。
- 个人统筹设计 AI Infra 场景下 NPU，Metax，Nvidia 等异构算力资源纳管、平台适配与模型服务接入，支撑算力集群落地及对外服务能力建设。
- 在客户现场及交付过程中，沉淀标准化部署、升级、排障与运维流程，提升复杂环境下平台交付效率与稳定性。

## **项目经历**
## **云原生 AI / 大模型基础设施实践**
#### **主要负责内容**
- 面向 **4** 套集群、三类异构算力场景，参与建设 AI Infra 基础设施与模型服务接入能力，覆盖 **Nvidia,Metax,NPU** 等算力资源的统一纳管与平台适配。
- 多集群统一纳管方案落地,支撑3套算力集群接入与资源管理,提升异构环境下的统一运维与交付效率。
- 主导设计vGPU 使用方案,统筹原生开源组件Ascend-mindxl,GPU Operator,HAMI等组件规范集群的GPU管理,适配与问题排查,支撑共享能力,如**sGPU,vNPU资源调度等能力**落地,提升资源使用灵活性与利用率。
- 设计并落地统一模型服务接入方案,对外暴露 **30+** 个模型服务,**提供标准化接口能力**,并**结合网关实现基于鉴权方式的访问控制与服务隔离**。
- 基于Cert-Manager建设模型服务 TLS 证书签发与生命周期管理能力,支撑**10**个对外服务的安全接入,完善模型服务暴露链路。
- 结合 Service Mesh,Gateway API,Kyverno + NetWorkPolicy 实现**东西南北的流量治理与访问控制**,提升模型服务安全性与可控性。
- 处理并推动解决兼容性,适配类关键问题,包括典型问题，**如vLLM 适配,NPU 驱动兼容,GPU 共享调度,推理链路接入,证书与网关联调**。

## **云原生可观测体系建设**
#### **主要负责内容**
- 面向**10套集群**、**96+业务场景**，建设统一可观测平台，打通日志、指标与链路追踪能力。
- 参与设计并落地基于 Fluent Bit → Kafka → Vector → Elasticsearch / Kibana 的日志链路,支撑 **日均2TB**，**会员日峰值6TB规模**的数据采集、传输、缓冲与检索。
- 推动以 OpenTelemetry 作为统一观测协议落地，兼容SkyWalking Java Agent，支撑**96+服务/4类不同语言类型应用**的链路采集与平滑迁移。
- 参与 SkyWalking 向 OpenTelemetry 的迁移与**数据聚合改造**，**处理5+项采集兼容、字段映射、链路连续性及数据一致性问题**。
- 参与 Kafka 日志链路跨环境迁移与稳定性治理，处理**12+项消费延迟**、链路堆积、缓冲异常、迁移一致性等问题，保障日志链路稳定运行。

## **云原生网关与服务治理**
#### **主要负责内容**
- 面向**10套集群**、**96+业务场景**,参与建设基于 Contour + Envoy 的云原生网关体系,支撑服务统一接入与入口流量治理。
- 参与基于 HTTPProxy / Ingress 的路由配置管理能力建设,**支撑 36 个域名**、**86 个服务**的对外暴露与流量转发。
- 设计并实施网关数据面健康监控与观测方案,覆盖**12个**数据面实例/**4套**环境,提升网关链路稳定性与故障定位效率。
- 打通 Envoy 到 OpenTelemetry / 后端观测系统的数据采集链路,支撑链路类型等观测数据接入,增强流量治理与问题排查能力。
- 处理**5项**网关接入、路由配置、证书联调、流量转发或观测链路**相关问题**,支撑生产环境网关稳定运行。

## **云原生中间件集群建设与运维**
#### **主要负责内容**
- 向**2家**客户,**31个**业务场景,参与云原生中间件集群建设与运维实践,覆盖 Redis、RabbitMQ、RocketMQ、Kafka、Elasticsearch、MySQL、PostgreSQL 等核心组件。
- 参与**1套跨数据中心的中间件集群**的部署、升级、扩缩容、配置优化与高可用维护,支撑缓存、消息、检索与数据库类服务稳定运行。
- 累计处理**13余项生产故障与专项问题**,涉及**消息中间件堆积,消息持久化,Cache回收,内部证书更新,开源BUG**等场景，提升中间件平台稳定性与问题闭环效率。
- 面向业务交付与生产变更场景，支撑**23+次中间件升级、迁移或架构调整**，保障变更过程平稳可控。

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
  具备较强的云原生基础设施实践能力，技术方向覆盖容器平台、可观测、中间件、网关治理及异构算力等多个领域，知识面较完整，工程落地能力较强。能够在多集群、复杂生产环境下承担平台交付、问题排查、方案推进和稳定性保障相关工作，对系统性问题有一定分析与收敛能力。整体偏向工程实践型，既能参与方案建设，也能深入一线处理实际问题。

