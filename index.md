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
[**深圳前海道客网络科技有限公司 - 南区交付 - 运维交付**](https://www.daocloud.io/) `2024/7-至今`
+ 负责公司产品的交付和公司产品的维护保证
+ 负责自动化运维组件的部署
+ 处理containerd，kubernetes等容器和容器编排问题
+ 处理集群中服务部署的环境问题以及处理兼容性问题。

[**华南理工大学广州学院 - 机房教学中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021/9-2025/6`

+ 管理语音教学中心的6台linux服务器，保证日常99%时间的平稳运行
+ 深度涉及云服务管理，自动化运维，系统管理，网络管理，服务器管理等。维护多种教学系统的运行。
+ 实现应用程序容器化部署，并使用Kubernetes完成容器部署的编排工作。

[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

+ 熟练掌握并应用Ansible自动化运维工具，实现自动化部署、配置管理及环境监控。
+ 利用Docker和Kubernetes，有效管理和部署容器化应用，提高部署速度、扩展性及系统资源利用率。
+ 实施高级监控解决方案如Prometheus，进行系统和网络性能监控


## 项目经历   

### **KafKa跨机房集群的数据双向同步** 中间件架构工程师 `2024/12-2025/1`
 负责 Kafka 集群双向同步方案的设计与落地，针对跨集群数据同步场景，通过 MirrorMaker 2 配置优化、消息打标防环、时间戳冲突处理、分区并行优化等手段，解决了数据一致性、回环问题、性能延迟等核心痛点；同时结合 ACL 同步工具、Checkpoint 机制和监控告警体系，保障了数据零丢失、顺序一致性以及权限同步，成功支持了双活架构、跨地域数据复制及云迁移等高可用场景，提升了系统的稳定性和业务连续性。

### **Rocketmq中间件高可用方案** 中间件架构工程师 `2024/10-2024/11`
  基于 Kubernetes Operator 部署 RocketMQ 集群，通过 StatefulSet 实现 Namesrv 和 Broker 多副本高可用，结合 LocalPV 持久化存储保障数据可靠性，针对 Operator 缺陷（Namesrv 副本/IP 变更触发滚动重启），重构 Broker 配置（allowRestart: false）规避生产风险。对比 Calico IPAM 固定分配、MetalLB LoadBalancer IP 预留、Macvlan CNI 直通等方案，最终采用 Macvlan 实现 Pod 级静态 IP 绑定，确保 Broker/Namesrv 节点 IP 在集群扩容、故障迁移等场景下永久不变。
  
### **集群网络方案** 架构交付 `2024/9-2024/10`
  通过部署 Cilium 网络插件并结合 BGP Underlay 模式，可以实现跨集群的 Pod 网络互通和动态服务发现。Cilium利用eBPF技术提供高效的流量转发和细粒度的安全策略，而BGP协议则确保了外部网络与集群间的动态路由更新，使得Pod IP及服务类型能被实时通告。这样，集群间的Pod可以无缝互访，同时动态注册的服务能够被外部网络识别并访问。此外，Cilium的网络性能优化、流量聚合以及对L7策略的支持，使得云原生应用的网络更加安全、灵活和可管理，充分满足了复杂场景下的性能和可扩展性需求。
  
### **容器云平台devops/CICD** 云原生DevOps工程师 `2024/08-2024/09`
 基于Jenkins设计并实现CI/CD流水线，集成GitOps（FluxCD）与Argo工具链，使用Jenkins Pipeline构建声明式流水线，集成Trivy镜像扫描、优化镜像体积、SonarQube代码质量分析，确保交付安全与质量。通过Argo Rollouts实现金丝雀发布与蓝绿部署，结合Prometheus指标自动判断发布状态，支持失败自动回滚，采用GitOps实践，使用FluxCD同步Git仓库配置至Kubernete集群，实现基础设施即代码（IaC）。

### **kubevirt存储验证** 技术测试工程师 `2024/08-2024/09`
 集群KubeVirt的VM测试包括，镜像创建，yaml创建，克隆，实时迁移，创建快照，快照备份，CPU内存更新，各种网络模式，hwameistor和ceph存储io性能测试，跨集群迁移，vmdk导入。特殊离线环境下，修改ubuntu版本的fio专用编译包，然后进行离线编译fio工具，创建进行存储测试对比，对比随机写，随机读，随机混合读写，顺序读，顺序写的fio测试参数。便携数据分析python脚本进行多次测试的可视化分析，输出特定环境的测试文档。
 
### **容器管理定制化交付** 容器交付工程师 `2024/07-2024/08`
 主导生产集群升级方案，在离线环境下自建三副本Harbor镜像仓库，实现镜像版本统一管理和灾备。解构官方Chart包，重构NodePort服务暴露方式，优化Ingress路由配置，适配探针策略，针对NFS存储环境，定制容器目录权限方案，解决MySQL容器因权限问题导致的CrashLoopBackOff故障，通过存储动态扩容+重挂载方案，确保服务容器可用性达99%。

### **高可用云原生架构搭建**   云架构师   `2022/04-2022/06`
  基于AWS构建千万级流量支撑架构，采用双可用区部署策略，通过公有子网（对接互联网网关）+私有子网（通过NAT网关通信）实现业务隔离。网络ACL实现子网级流量管控，安全组细化到实例端口权限，堡垒机统一运维入口，使用CloudFormation自动化部署VPC集群，结合Auto Scaling实现业务流量30%弹性扩容，Redis缓存热点数据使接口响应提升50%，SQS解耦核心业务模块，DynamoDB分布式会话存储并发稳定性。

### **个人博客**  独立开发者  `2021/09-2024/05`
  基于Hexo+Node.js搭建静态博客，利用其秒级编译和插件生态，实现90%文章「Markdown写稿+Git版本管理+自动发布」一条龙，用EJS模板重写页面结构，手搓响应式布局适配手机/平板，添加全局搜索、友链特效等实用功能，通过Vercel自动化部署，配合CDN加速和HTTPS证书，页面加载速度稳定。
  

  
  
## 相关技能
1. **计算机网络**：TCP/IP, HTTP, DNS, WebSocket, RPC
2. **操作系统**：CentOS, Ubuntu, RHEL, Windows,almaLinux
3. **自动化运维工具**：Ansible
4. **可观测技术**：Prometheus, Grafana, Kibana，OpenTelemetry，Victoriametrics，fluentbit
5. **微服务**：Envoy,Istio
6. **DevOps**：Jenkins
7. **中间件**：Kafka,RocketMQ,Elasticsearch,Redis,MySQL,PostgreSQL,RabbitMQ，
8. **容器化**：Containerd, Docker，podman
9. **容器编排**：Kubernetes
10. **镜像管理**：Harbor,jfrog
11. **集群技术**：Kubevirt,Kubean,Kind,MetalLB,Kubespray,helm
12. **网络技术**：Calico,Cilium
13. **编程技术**：Golang,Java,python

## 个人总结
  对kubernetes生态较为熟悉，容器化技术和容器编排工具经验丰富，熟悉多种集群技术，能够编写自动化脚本，具备网络基础知识，熟悉使用自动化运维工具，掌握不同发行版的Linux系统，掌握基本开发能力。

