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
  url: 
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
    - phone
-->

{% include cv-contact.html %}

## 教育经历

### 华南理工大学广州学院 本科 计算机学院 软件工程 `2021-至今`

## 工作经验

[**华南理工大学广州学院 - 机房教学中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021-2025`

+ 管理语音教学中心的6台linux服务器，保证日常99%时间的平稳运行
+ 深度涉及云服务管理，自动化运维，系统管理，网络管理，服务器管理等。维护多种教学系统的运行。
+ 实现应用程序容器化部署，并使用Kubernetes完成容器部署的编排工作。

[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

+  熟练掌握并应用Ansible、Puppet、Terraform等自动化运维工具，实现自动化部署、配置管理及环境监控。
+ 利用Docker和Kubernetes，有效管理和部署容器化应用，提高部署速度、扩展性及系统资源利用率。
+ 实施高级监控解决方案如Prometheus和Grafana，进行系统和网络性能监控，以及利用ELK Stack进行日志分析，增强对系统运行状态的可视化和问题预警能力。



## 项目经历
### 社会项目
#### **智能教学环境集成系统**  `2022/09-2023/04`
  我在语言教学中心的机房担任运维工作，成功实施了一套综合性的智能教学环境集成系统。利用VMware vSphere和VirtualBox进行高效的虚拟化管理，同时部署了Ansible和Puppet以自动化系统的配置，确保了高度的一致性和可靠性。通过Jenkins和GitLab CI/CD，我有效实现了代码的自动部署和连续集成，提升了教学软件的迭代速度和稳定性。网络方面，我采用Cisco软件和Wireshark进行精准的流量监控和管理，确保网络安全和性能。此外，通过部署Prometheus和Grafana以及集成Alertmanager，我建立了全面的监控和实时告警系统。安全加固方面，通过配置iptables和pfSense以及运用Snort或Suricata的入侵检测系统，我强化了整体网络的防护能力。这一系列技术的应用大大提高了系统的稳定性和教学的效率，展现了我在信息技术管理和优化方面的专业能力。

### 个人项目
#### **仿无影无服务器云架构** 
  我对云计算及其架构产生了强烈的兴趣，尤其是在无服务器计算和容器化方面。为了深入探索这些领域，我启动并实施了一个模拟阿里云无影架构的个人项目，采用AWS服务完成。在这个项目中，我熟练地运用AWS Lambda来执行事件驱动的计算任务，无需管理服务器。通过Amazon API Gateway，我构建和部署了安全且可伸缩的API接口。同时，我利用Amazon ECS和AWS Fargate部署容器化应用，实现服务和集群的自动化管理。项目还包括部署Amazon Aurora Serverless和Amazon DynamoDB以提供自动伸缩的数据库服务，以及使用Amazon S3和Amazon CloudFront进行高效的文件存储和内容分发。此外，我借助AWS CloudFormation和AWS CDK自动化云资源管理，整合AWS CodePipeline与AWS CodeBuild实现代码的持续集成和部署。性能监控方面，我部署了Amazon CloudWatch和AWS X-Ray以优化系统监控和服务追踪。为增强安全性，我配置了AWS IAM、Amazon Cognito、AWS WAF和AWS Shield，确保应用的安全性和合规性。这个项目不仅加深了我的技术理解，也显著提升了我的云计算实践能力。

#### **高可用弹性B/S架构**

  搭建了一个详细的虚拟私有云（VPC）架构，包含多个AWS组件和服务。该架构包括一个名为"MyVPC"的VPC，内部包含多个子网（如PublicSubnetA、PublicSubnetB、PrivateSubnetA、PrivateSubnetB）和路由表（如PublicRouteTable、PrivateRouteTable）。此外，还配置了网络ACL（如PublicNetworkACL、PrivateNetworkACL）来控制子网的入站和出站流量。网络设备方面，包含一个InternetGateway用于公共子网的互联网访问，以及一个NATGateway和其对应的弹性IP用于私有子网的互联网访问。安全组（如PublicInstanceSecurityGroup、PrivateInstanceSecurityGroup）用于实例的流量控制。实例部分，包括PublicInstanceA、PublicInstanceB、PrivateInstanceA、PrivateInstanceB等。该架构使用堡垒机来登录实例，VPC通过CloudFormation模板构建，并基于CloudWatch指标实现自动扩展（AutoScaling）。会话状态保存在DynamoDB中，数据库缓存使用Amazon ElastiCache for Redis。此外，还使用消息队列SQS来处理消息。这些组件通过复杂的连接关系，构成了一个集成的、高度可扩展和可靠的网络架构，用于管理和控制流量的路由、访问和安全性，适用于在云环境中部署和管理各种应用和服务。

## 相关技能
1.熟悉主流云服务提供商AWS的服务和管理工具，以及常用架构的搭建能力。

2.熟练使用容器化技术和容器编排工具，Docker和Kubernetes。

3.能够编写自动化脚本，熟悉脚本语言，如Python、Bash

4.了解持续集成和持续部署（CI/CD）流程，以及相关工具Jenkins、GitLab CI。

5.具备网络基础知识，包括TCP/IP、DNS、HTTP/HTTPS以及负载均衡器。

6.掌握以下自动化运维工具的使用Ansible

7.熟悉Linux系统管理，包括系统安装、配置、监控和性能优化。

## 个人总结
  对DevOps职位的具体工作流程和相关工具具有扎实的理解，并通过项目和课程实践积累了相应的使用经验。我熟悉主流云服务平台如AWS的基本功能和架构搭建技术，了解微服务架构的基础，并掌握了Docker等容器化技术以及Kubernetes等容器编排工具的使用。此外，我对Linux操作系统和网络基本知识有深入了解，并通过学习和实验室项目，熟悉了Ansible等自动化运维工具的基础运用。正处于学习和成长阶段的我，渴望通过实习机会，将这些理论知识和基本技能运用于实际工作中，以进一步提升自己的专业能力和工作经验。



## 证书奖项
- AWS Certified Solutions Architect -Associate（SAA）认证
- CNCF Certified Kubernetes Administrator(CKA) 认证
- OceanBase CA专员认证
