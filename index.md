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

### 广州城市理原华南理工大学广州学院 本科 软件工程 `2021-至今`

## 工作经验

[**华南理工大学广州学院 - 机房语音教学中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021-2025`

本人作为运维组组长，管理语音教学中心的700+台网络设备，深度涉及云服务管理，自动化运维，系统管理，网络管理，服务器管理等。维护多种教学系统的运行。



[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

在机器人实验室软件组，我深度学习了对云计算架构的理解，并通过编写自动化运维脚本，有效提升了系统的稳定性和运行效率。



## 项目经历


### **智能教学环境集成系统** *语言教学中心* `2022/09-至今`

开始进行语言教学中心的机房运维工作后，学校日常考试教学需要进行系统的搭建和维护，为了尽快在多台计算机中搭建系统环境，和服务器的管理环境，我采取了以下行动：


接手运维工作后，发现原有运维架构存在权限管理粗放、业务部署混乱、应用配置变更困难、服务可靠性差等问题。为提高业务与基础设施的可用性与稳定性，我采取了以下措施：

- 回收所有服务器与数据库权限，并依据最小权限原则进行权限再分配，为服务器集群开发和建设了基于CA的ssh登录认证体系，结束了权限管理粗放的问题。
- 建设团队私有kubernetes集群，依据Google Borg论文对各类存量服务整理、分类和改造并逐步迁移至集群中，从而保证基础设施的标准统一与部署规范。
- 以gitlab-ci为中心，结合ansible、helm等工具推进gitops体系建设，允许以声明式配置对nginx、sshd、k8s等基础设施进行变更，从而保证了业务迭代的敏捷与配置变更的规范。
- 围绕kube-prometheus-stack与grafana-stack，建设包含监控、日志、链路追踪、性能分析的全链路可观测平台，为业务和基础设施提供完整的可观测能力和基本的告警能力，在为业务开发提供便利便利的同时，将故障发现时间由数小时缩减到五分钟内，进而大幅提升服务可靠性。
- 通过主动发现业务异常和及时响应报警，解决过多起线上事故。并在事后通过复盘、整理、归纳并优化相关问题，最终将整个团队的故障频率由每月10次以上降低到2次以下。

## 相关技能

- 编程语言：能熟练编写bash与python脚本，可以使用Go与C进行中间件和底层组件开发，可以使用vue进行前端开发。
- 操作系统：使用Arch Linux作为日常使用的操作系统，拥有个人维护的[AUR包](https://aur.archlinux.org/packages?O=0&SeB=m&K=kawhicurry&outdated=&SB=m&SO=d&PP=50&submit=Go)。了解systemd，ebpf。
- 性能分析：了解性能分析的基本方法与工具，能熟练使用sysstat、ebpf工具对系统性能问题进行分析。
- 语言能力：良好的中英语阅读能力与文档编写能力。
- 其他能力：了解SRE的基本观念，有标准化意识，有主动发现与解决问题的能力

## 证书奖项

- AWS Certified Solutions Architect -Associate
- CNCF Certified Kubernetes Administrator(CKA) 认证
