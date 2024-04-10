---
layout: cv
title: Kalyan's Resume
email:
  url: mailto:kalyan.zitiu@gmail.com
  text: kalyan.zitiu@gmail.com
homepage:
  url: https://www.kalyan.life
  text: kalyan.life
---

# 黄梓涛

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

[**华南理工大学广州学院 - 机房教学中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021-2025`

+ 管理语音教学中心的6台linux服务器，保证日常99%时间的平稳运行
+ 深度涉及云服务管理，自动化运维，系统管理，网络管理，服务器管理等。维护多种教学系统的运行。
+ 实现应用程序容器化部署，并使用Kubernetes完成容器部署的编排工作。



[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

+ 掌握了对云计算架构的理解，并通过编写自动化运维脚本，有效提升了服务器系统的稳定性和运行效率。
+ 掌握自动化运维工具，对服务器进行自动化部署



## 项目经历
### 社会项目
#### **智能教学环境集成系统**  `2022/09-2023/04`
开始进行语言教学中心的机房运维工作后，学校日常考试教学需要进行系统的搭建和维护，为了尽快在多台计算机中搭建系统环境，和服务器的管理环境，我采取了以下技术
虚拟化技术：我利用VMware vSphere和VirtualBox容器技术来创建和管理虚拟化的教学环境，使得资源可以按需分配，并且可以快速复制和恢复系统状态。
配置管理：我部署了Ansible和Puppet来自动化配置管理，确保所有机器的配置一致性和可复制性，同时大幅降低了手动配置的错误率和维护时间。
持续集成/持续部署 (CI/CD)：通过Jenkins和GitLab CI/CD管道，我实现了自动化的代码部署和测试流程，确保了教学软件的快速迭代和稳定性。
网络管理：我使用了高级网络工具如Cisco的网络管理软件和Wireshark来监控网络流量，及时发现并解决网络瓶颈和安全隐患。
监控和告警：我部署了Prometheus和Grafana来监控系统和网络性能指标，结合Alertmanager进行实时告警，确保能够快速响应潜在的系统问题。
安全加固：使用防火墙技术（如iptables和pfSense），以及入侵检测系统（如Snort或Suricata）

### 个人项目
#### **仿无影无服务器云架构** 
在掌握了语言教学中心机房运维工作的基础上，我开始对云计算架构产生浓厚的兴趣，特别是在无服务器计算和容器化方面。为了深入学习并实践这些概念，我启动了一个模拟阿里云无影架构的个人项目，采用了AWS服务进行实现。主要技术和策略包括：
无服务器计算和API管理：
利用AWS Lambda实现事件驱动的计算任务，无需预置或管理服务器。
通过Amazon API Gateway构建和部署安全、可扩展的API接口。
容器化服务和无服务器部署：
使用Amazon ECS和AWS Fargate来运行容器化应用，实现了服务器和集群管理的自动化。
自动化数据库服务：
部署Amazon Aurora Serverless数据库，根据实际负载自动调整计算能力，优化成本。
使用Amazon DynamoDB作为高可用性和无服务器的键值及文档数据库。
文件存储和全球内容分发：
采用Amazon S3进行对象存储，实现了数据的高可靠性和可扩展性。
结合Amazon CloudFront提供快速的内容分发网络服务，优化全球用户的访问速度。
基础设施即代码和CI/CD：
利用AWS CloudFormation和AWS CDK自动化云资源的创建和管理。
集成AWS CodePipeline和AWS CodeBuild，实现代码的持续集成和持续部署。
性能监控和日志分析：
部署Amazon CloudWatch和AWS X-Ray进行应用和基础设施的监控，以及服务调用追踪。
安全性和合规性：
使用AWS IAM和Amazon Cognito进行访问控制和用户身份验证。
配置AWS WAF和AWS Shield强化Web应用的安全性。

## 相关技能
1.熟悉主流云服务提供商（如AWS）的服务和管理工具，以及常用架构的搭建能力。

2.熟练使用容器化技术和容器编排工具，如Docker和Kubernetes。

3.能够编写自动化脚本，熟悉脚本语言，如Python、Bash

4.了解持续集成和持续部署（CI/CD）流程，以及相关工具，如Jenkins、GitLab CI。

5.具备网络基础知识，包括TCP/IP、DNS、HTTP/HTTPS以及负载均衡器。

6.掌握以下自动化运维工具的使用，Ansible，Chef，Puppet

## 个人总结
+ 我熟练使用java，python，Kotlin等编程语言，并擅长开发用其开发项目以解决生活实际问题
+ 我对Web前端和框架较为熟悉，而且有一定兴趣，能够编写较好交互的良好网站，并且有自己维护的技术博客kalyan.life
+ 熟悉DevOps职位具体工作的流程和工具，掌握主流云服务的功能以及基本搭建能力

## 证书奖项
- AWS Certified Solutions Architect -Associate（SAA）认证
- CNCF Certified Kubernetes Administrator(CKA) 认证
- OceanBase CA专员认证
