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
[**深圳前海道客网络科技有限公司 - 南区交付 - 运维交付**]
+ 负责公司产品的交付和公司产品的维护保证
+ 负责自动化运维组件的部署
+ 处理containerd，kubernetes等容器和容器编排问题 

[**华南理工大学广州学院 - 机房教学中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021-2025`

+ 管理语音教学中心的6台linux服务器，保证日常99%时间的平稳运行
+ 深度涉及云服务管理，自动化运维，系统管理，网络管理，服务器管理等。维护多种教学系统的运行。
+ 实现应用程序容器化部署，并使用Kubernetes完成容器部署的编排工作。

[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

+  熟练掌握并应用Ansible自动化运维工具，实现自动化部署、配置管理及环境监控。
+ 利用Docker和Kubernetes，有效管理和部署容器化应用，提高部署速度、扩展性及系统资源利用率。
+ 实施高级监控解决方案如Prometheus，进行系统和网络性能监控


## 项目经历

### **创信合金DaoCloud容器云平台** 交付人员 `2024/07-至今`
 与创信合金合作共同完成Daocloud容器云平台，搭建集成了服务网格和微服务技术，支持多云和边缘云管理，提供多云编排、容器管理、微服务治理、DevOps 支持等功能，能够实现应用交付过程的标准化和自动化理的高性能、可扩展的云原生操作系统，对生产集群进行更好的监控和生产操作。

### **智能教学环境集成系统**    项目实施人   `2022/09-2023/04`
  我在语言教学中心的机房担任运维工作，成功实施了一套综合性的智能教学环境集成系统。利用高效的虚拟化管理，同时部署了Ansible以自动化系统的配置，确保了高度的一致性和可靠性。通过Jenkins，我有效实现了代码的自动部署和连续集成，提升了教学软件的迭代速度和稳定性。此外，通过部署Prometheus，我建立了全面的监控和实时告警系统。

### **个人博客**     开发人员   `2021/09-2024/05`
  这个项目是一个个人技术博客，旨在分享我的编程知识、技术心得以及个人项目经验。它基于 Node.js ，拥有极快的生成速度，以及丰富的插件系统，能够轻松扩展功能。文章使用 Markdown 语法编写，这不仅便于内容的快速撰写和格式化，还能通过版本控制工具如 Git 进行版本管理。利用 EJS 模板引擎对默认主题进行定制，包括布局调整、样式自定义以及添加新的功能组件。

### **高可用弹性B/S架构**   搭建人   `2024/04-2024/06`
  在AWS环境中构建的"MyVPC"虚拟私有云架构包括配置了多个公共和私有子网，分别通过与互联网网关和NAT网关相关联的路由表管理互联网访问，确保流量安全和隔离。网络安全依靠具体设定的网络ACL和针对公共及私有实例的安全组来精确控制入站和出站流量。系统采用堡垒机进行安全登录与实例管理，而整个VPC的部署和管理通过CloudFormation模板实现自动化，同时支持自动扩展功能以便根据需要调整资源。会话状态的管理借助DynamoDB实现，而数据访问速度通过使用Amazon ElastiCache for Redis进行加速。此外，引入消息队列SQS来优化应用间的异步通信，整体上，这套架构有效地提供了一个高度集成、可扩展且安全的网络环境，适用于云上的多种应用和服务部署。
  

## 相关技能
1.熟练使用容器化技术和容器编排工具，Docker，Containerd和Kubernetes。

2.熟悉多种集群技术，包括不限于envoy，istio，calico，cilium，hwameistor，KafKa,RocketMQ,Redis,Elasticsearch，kubevirt，kubean，kind等

3.能够编写自动化脚本，熟悉脚本语言，如Python、Bash

4.具备网络基础知识，包括不限于TCP/IP、DNS、HTTP/HTTPS，RPC，Websocket.

5.熟悉使用自动化运维工具ansible进行多hosts的维护以及生产操作。

6.熟悉不同发行版的Linux系统以及linux内核，掌握Linux以及众多工具的使用以及操作

7.熟悉CICD，jinkens流水线，GitOps等Devops运维技术。


## 个人总结
  对kubernetes生态较为熟悉，能够建立并且维护自建集群，能够使用多种集群技术对集群进行多维度操作，包括不限于组件升级。熟悉linux操作系统，对不同发行版有不同的研究和理解。对不同的技术能够快速进行学习以及实操上手。

