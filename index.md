---
layout: cv
title: Kalyan's Resume
email:
  url: mailto:kalyan.zitiu@gmail.com
  text: kalyan.zitiu@gmail.com
homepage:
  url: https://blog.zitiu.top/
  text: kalyan.life
phone:
  text: 19866803602
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
[**深圳前海道客网络科技有限公司 - 南区交付 - 运维交付**](https://www.daocloud.io/) `2024/7-2024/12`
+ 负责公司产品的交付和公司产品的维护保证
+ 负责自动化运维组件的部署
+ 处理containerd，kubernetes等容器和容器编排问题
+ 处理集群中客户服务部署的环境问题以及处理兼容性问题。

[**华南理工大学广州学院 - 机房教学中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021/9-2025/6`

+ 管理语音教学中心的6台linux服务器，保证日常99%时间的平稳运行
+ 深度涉及云服务管理，自动化运维，系统管理，网络管理，服务器管理等。维护多种教学系统的运行。
+ 实现应用程序容器化部署，并使用Kubernetes完成容器部署的编排工作。

[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

+ 熟练掌握并应用Ansible自动化运维工具，实现自动化部署、配置管理及环境监控。
+ 利用Docker和Kubernetes，有效管理和部署容器化应用，提高部署速度、扩展性及系统资源利用率。
+ 实施高级监控解决方案如Prometheus，进行系统和网络性能监控


## 项目经历

### **安踏体育网络方案** 架构交付 `2024/10-2024/11`
  在集群中部署并配置Cilium网络插件，结合BGP Underlay模式启用BGP控制平面和Peering，将Pod IP及各种Service类型通过BGP通告到外部网络，实现跨集群Pod的无缝互访、动态服务注册与发现，以及直接对Pod进行调试，同时充分利用Cilium的最新特性以优化网络性能、增强安全性并提升整体可管理性，从而满足复杂多变的云原生应用需求。

### **屈臣氏中国-Daocloud-VM存储验证** 交付人员 `2024/08-2024/09`
 集群KubeVirt的VM测试包括，镜像创建，yaml创建，克隆，实时迁移，创建快照，快照备份，CPU内存更新，各种网络模式，hwameistor和ceph存储io性能测试，跨集群迁移，vmdk导入。特殊离线环境下，修改ubuntu版本的fio专用编译包，然后进行离线编译fio工具，创建进行存储测试对比，对比随机写，随机读，随机混合读写，顺序读，顺序写的fio测试参数。便携数据分析python脚本进行多次测试的可视化分析，输出特定环境的测试文档。

### **创金合信-DaoCloud容器云平台** 交付人员 `2024/07-2024/08`
 与创信合金合作共同完成Daocloud容器云平台，搭建集成了服务网格和微服务技术，支持多云和边缘云管理，提供多云编排、容器管理、微服务治理、DevOps 支持等功能，能够实现应用交付过程的标准化和自动化理的高性能、可扩展的云原生操作系统，对生产集群进行更好的监控和生产操作。对集群内组件进行镜像升级，建立流水线操作进行仓库拉取，镜像维护后，对其进行流水线+流水线执行id+时间戳的版本跟踪的构建并且推送至组件拉取的镜像仓库。

### **珠海翔翼软件实施** 交付人员 `2024/08-2024/09`
 升级珠海翔翼生产集群的服务镜像版本升级，以及正式服务部署。离线环境下，搭建三副本harbor仓库进行镜像存储管理以及制作环境专用的helm chart进行实际部署。基于特殊存储环境进行容器环境目录权限授权，以及部署后容器存储扩容和重新挂载，保证服务容器日常99%正常运行。通过拉取官方服务的helm chart进行解包修补，修改NodePort服务类型以及镜像路径和版本，配置具体ingress，以及探针参数。修改bitnami mysql container的values的配置，避免出现目录下操作无权限导致crashloopbackoff问题。

### **智能教学环境集成系统**    项目实施人 `2022/09-2023/04`
  我在语言教学中心的机房担任运维工作，成功实施了一套综合性的智能教学环境集成系统。利用高效的虚拟化管理，同时部署了Ansible以自动化系统的配置，确保了高度的一致性和可靠性。通过Jenkins，我有效实现了代码的自动部署和连续集成，提升了教学软件的迭代速度和稳定性。此外，通过部署Prometheus，我建立了全面的监控和实时告警系统。

### **个人博客**     开发人员 `2021/09-2024/05`
  这个项目是一个个人技术博客，旨在分享我的编程知识、技术心得以及个人项目经验。它基于 Node.js ，拥有极快的生成速度，以及丰富的插件系统，能够轻松扩展功能。文章使用 Markdown 语法编写，这不仅便于内容的快速撰写和格式化，还能通过版本控制工具如 Git 进行版本管理。利用 EJS 模板引擎对默认主题进行定制，包括布局调整、样式自定义以及添加新的功能组件。
  
### **高可用弹性B/S架构**   搭建人   `2024/04-2024/06`
  在AWS环境中构建的"MyVPC"虚拟私有云架构包括配置了多个公共和私有子网，分别通过与互联网网关和NAT网关相关联的路由表管理互联网访问，确保流量安全和隔离。网络安全依靠具体设定的网络ACL和针对公共及私有实例的安全组来精确控制入站和出站流量。系统采用堡垒机进行安全登录与实例管理，而整个VPC的部署和管理通过CloudFormation模板实现自动化，同时支持自动扩展功能以便根据需要调整资源。会话状态的管理借助DynamoDB实现，而数据访问速度通过使用Amazon ElastiCache for Redis进行加速。此外，引入消息队列SQS来优化应用间的异步通信，整体上，这套架构有效地提供了一个高度集成、可扩展且安全的网络环境，适用于云上的多种应用和服务部署。

  
  
## 相关技能
1. **计算机网络**：TCP/IP, HTTP, DNS, WebSocket, RPC
2. **操作系统**：CentOS, Ubuntu, RHEL, Windows,almaLinux
3. **自动化运维工具**：Ansible
4. **可观测技术**：Prometheus, Grafana, Kibana，Loki
5. **微服务**：Envoy,Istio
6. **DevOps**：Jenkins
7. **中间件**：Kafka,RocketMQ,Elasticsearch,Redis,MySQL,PostgreSQL,Redis
8. **容器化**：Containerd, Docker，podman
9. **容器编排**：Kubernetes
10. **容器管理**：Harbor,jfrog
11. **集群技术**：Kubevirt,Kubean,Kind,MetalLB,Kubespray,helm
12. **网络技术**：Calico,Cilium
13. **编程技术**：Golang,Java,python

## 个人总结
  对kubernetes生态较为熟悉，容器化技术和容器编排工具经验丰富，熟悉多种集群技术，能够编写自动化脚本，具备网络基础知识，熟悉使用自动化运维工具，掌握不同发行版的Linux系统，掌握基本开发能力。

