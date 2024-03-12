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

### 华南理工大学广州学院 本科 软件工程 `2021-至今`

## 工作经验

[**华南理工大学广州学院 - 机房语音教学中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021-2025`

本人作为运维组组长，管理语音教学中心的700+台网络设备，深度涉及云服务管理，自动化运维，系统管理，网络管理，服务器管理等。维护多种教学系统的运行。



[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

在机器人实验室软件组，我深度学习了对云计算架构的理解，并通过编写自动化运维脚本，有效提升了系统的稳定性和运行效率。



## 项目经历


### **智能教学环境集成系统** *语言教学中心* `2022/09-至今`

开始进行语言教学中心的机房运维工作后，学校日常考试教学需要进行系统的搭建和维护，为了尽快在多台计算机中搭建系统环境，和服务器的管理环境，我采取了以下技术

虚拟化技术：我利用VMware vSphere和VirtualBox容器技术来创建和管理虚拟化的教学环境，使得资源可以按需分配，并且可以快速复制和恢复系统状态。

配置管理：我部署了Ansible和Puppet来自动化配置管理，确保所有机器的配置一致性和可复制性，同时大幅降低了手动配置的错误率和维护时间。

持续集成/持续部署 (CI/CD)：通过Jenkins和GitLab CI/CD管道，我实现了自动化的代码部署和测试流程，确保了教学软件的快速迭代和稳定性。

网络管理：我使用了高级网络工具如Cisco的网络管理软件和Wireshark来监控网络流量，及时发现并解决网络瓶颈和安全隐患。

集中日志管理：通过ELK Stack（Elasticsearch, Logstash, and Kibana）或者Graylog，我实现了日志的集中管理和分析，提高了问题诊断的效率。

监控和告警：我部署了Prometheus和Grafana来监控系统和网络性能指标，结合Alertmanager进行实时告警，确保能够快速响应潜在的系统问题。

备份与灾难恢复：我实施了基于Veeam和rsync的备份解决方案，以及详细的灾难恢复计划，以保证数据的完整性和系统的快速恢复能力。

安全加固：使用了先进的防火墙技术（如iptables和pfSense），以及入侵检测系统（如Snort或Suricata），并实行了严格的安全策略和最佳实践，包括定期的漏洞扫描和修补流程。

## 相关技能

熟悉主流云服务提供商（如AWS）的服务和管理工具。

掌握虚拟化技术，包括VMware、Hyper-V或KVM。

熟练使用容器化技术和容器编排工具，如Docker和Kubernetes。

能够编写自动化脚本，熟悉脚本语言，如Python、Bash

了解持续集成和持续部署（CI/CD）流程，以及相关工具，如Jenkins、GitLab CI或Travis CI。

熟悉基础设施即代码（IaC）工具，如Terraform、Ansible或CloudFormation。

具备网络基础知识，包括TCP/IP、DNS、HTTP/HTTPS以及负载均衡器。

掌握系统监控、日志管理和报警工具，如Prometheus、Grafana、ELK Stack或Splunk。

理解安全最佳实践，包括网络安全、数据加密和访问控制。

具备故障排查和性能优化的能力，能够快速响应并解决生产环境问题。

## 证书奖项

- AWS Certified Solutions Architect -Associate
- CNCF Certified Kubernetes Administrator(CKA) 认证
