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

[**华南理工大学广州学院 - 机房教学中心 - 运维组组长**](https://wy.gcu.edu.cn/2023/0523/c768a150266/page.htm) `2021-2025`

+ 管理语音教学中心的6台linux服务器，保证日常99%时间的平稳运行
+ 深度涉及云服务管理，自动化运维，系统管理，网络管理，服务器管理等。维护多种教学系统的运行。
+ 实现应用程序容器化部署，并使用Kubernetes完成容器部署的编排工作。

[**华南理工大学广州学院 - 机器人野狼队 - 软件组组员**](https://gcubot.cn) `2022/10-2023/10`

+  熟练掌握并应用Ansible自动化运维工具，实现自动化部署、配置管理及环境监控。
+ 利用Docker和Kubernetes，有效管理和部署容器化应用，提高部署速度、扩展性及系统资源利用率。
+ 实施高级监控解决方案如Prometheus，进行系统和网络性能监控



## 项目经历
### **智能教学环境集成系统**    项目实施人   `2022/09-2023/04`
  我在语言教学中心的机房担任运维工作，成功实施了一套综合性的智能教学环境集成系统。利用高效的虚拟化管理，同时部署了Ansible以自动化系统的配置，确保了高度的一致性和可靠性。通过Jenkins，我有效实现了代码的自动部署和连续集成，提升了教学软件的迭代速度和稳定性。此外，通过部署Prometheus，我建立了全面的监控和实时告警系统。安全加固方面，通过配置iptables，强化了整体网络的防护能力。这一系列技术的应用大大提高了系统的稳定性和教学的效率，展现了我在信息技术管理和优化方面的专业能力。



### **个人博客**     开发人员   `2021/09-2024/05`
  这个项目是一个个人技术博客，旨在分享我的编程知识、技术心得以及个人项目经验。它基于 Node.js ，拥有极快的生成速度，以及丰富的插件系统，能够轻松扩展功能。文章使用 Markdown 语法编写，这不仅便于内容的快速撰写和格式化，还能通过版本控制工具如 Git 进行版本管理。利用 EJS 模板引擎对默认主题进行定制，包括布局调整、样式自定义以及添加新的功能组件。对博客进行了搜索引擎优化（SEO），包括合理的标题、描述、URL 结构以及使用 sitemap 插件来增强网站的可发现性。结合 Git Hooks 和 CI/CD 工具，实现了博客内容的自动化部署，每次提交更新后，博客能够自动构建并推送到服务器。




### **高可用弹性B/S架构**   搭建人   `2024/04-2024/06`

  在AWS环境中构建的"MyVPC"虚拟私有云架构包括配置了多个公共和私有子网，分别通过与互联网网关和NAT网关相关联的路由表管理互联网访问，确保流量安全和隔离。网络安全依靠具体设定的网络ACL和针对公共及私有实例的安全组来精确控制入站和出站流量。系统采用堡垒机进行安全登录与实例管理，而整个VPC的部署和管理通过CloudFormation模板实现自动化，同时支持自动扩展功能以便根据需要调整资源。会话状态的管理借助DynamoDB实现，而数据访问速度通过使用Amazon ElastiCache for Redis进行加速。此外，引入消息队列SQS来优化应用间的异步通信，整体上，这套架构有效地提供了一个高度集成、可扩展且安全的网络环境，适用于云上的多种应用和服务部署。


  
### **安卓开发新闻APP**       开发人员 `2024/03-2024/05`
  安卓开发新闻 app 是一个为 Android 平台设计的移动应用程序，旨在为用户提供实时新闻内容。应用程序通过集成第三方新闻 API 来获取各种新闻源的最新信息，并提供一个直观易用的用户界面来展示新闻文章。用户可以浏览不同类别的新闻，收藏喜欢的文章，并在离线时阅读存储在本地数据库中的内容。用 Android Studio 通过 Java和 XML 布局进行开发。通过 Retrofit或 OkHttp用于处理 HTTP 请求返回，用 Gson 解析 API 返回的 JSON 数据。图片用 Glide 异步加载网络图片Room Persistence Library作为 SQLite 的抽象层，以便更加便捷地进行数据持久化操作，使用动态代理模式，通过 Retrofit 构建 REST API 的客户端。JUnit和 Espresso 用于单元测试和 UI 测试.



## 相关技能
1.熟悉主流云服务提供商AWS的服务和管理工具，以及常用架构的搭建能力。
2.熟练使用容器化技术和容器编排工具，Docker和Kubernetes。
3.能够编写自动化脚本，熟悉脚本语言，如Python、Bash
4.具备网络基础知识，包括TCP/IP、DNS、HTTP/HTTPS以及负载均衡器。
5.掌握以下自动化运维工具的使用Ansible
6.熟悉Linux系统管理，包括系统安装、配置、监控和性能优化。



## 个人总结
  对DevOps职位的具体工作流程和相关工具具有扎实的理解，并通过项目和课程实践积累了相应的使用经验。我熟悉主流云服务平台如AWS的基本功能和架构搭建技术，了解微服务架构的基础，并掌握了Docker等容器化技术以及Kubernetes等容器编排工具的使用。此外，我对Linux操作系统和网络基本知识有深入了解，并通过学习和实验室项目，熟悉了Ansible等自动化运维工具的基础运用。正处于学习和成长阶段的我，渴望通过实习机会，将这些理论知识和基本技能运用于实际工作中，以进一步提升自己的专业能力和工作经验。


