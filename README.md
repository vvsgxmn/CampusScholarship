# 基于SpringBoot+Vue的校园奖助学金申请系统

![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) ![Vue3](https://img.shields.io/badge/-Vue3-grey?style=flat-square) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MyBatis](https://img.shields.io/badge/-MyBatis-000000?style=flat-square&logo=mybatis&logoColor=white) 

## 项目介绍

本系统是一款面向高校学生与资助业务管理员的奖助学金全流程办理平台，针对项目查询分散、困难认定与申报脱节、院系初审与学校终审缺少统一台账、评选公示与异议反馈滞后、资助发放进度不透明等问题，把奖助项目展示、家庭经济困难认定、奖助申报、两阶段评审、评选公示、异议申诉、资助发放台账和政策资讯整合到同一套前后端分离工程中。

系统采用 SpringBoot + Vue 架构，区分学生与管理员：学生端查询项目、办理困难认定与奖助申请、跟踪评审进度、查阅公示与政策、提交异议并查看发放记录；管理端在数据看板掌握运营指标，维护奖助项目与政策，完成困难审核、申请初审/终审、公示发布、申诉处理与发放台账办理。业务状态可追溯、材料可留存，适合作为毕设、课设与高校资助业务学习参考。

## 主要功能模块

- **用户认证与角色分流**：学生与管理员统一登录注册，JWT 鉴权；登录后按角色进入学生门户或资助管理控制台，路由与接口双重隔离
- **学生首页总览**：个人业务概况、快捷入口与待办提示，便于进入项目查询、认定、申请与公示等核心办理路径
- **奖助项目查询**：按关键字与类别筛选奖学金、助学金与专项补助，查看金额、名额、开放状态、申报期间与资格门槛
- **家庭经济困难认定**：按学年提交认定档次、家庭人口与收入、困难陈述及证明材料，跟踪审核结论与核定档次
- **奖助申请提交**：在项目卡片填写申报陈述与佐证材料，系统校验 GPA、困难资格与重复申报后生成申请编号
- **我的申请与进度跟踪**：查看院系初审、学校终审阶段进度与审核意见，待初审阶段支持撤回申请
- **评选公示与异议申诉**：查阅公示正文与入围名单，对名单提交异议事由与举证材料，跟踪调查反馈
- **资助发放台账**：学生查看本人发放状态、金额与流水；管理员同步终审通过申请并办理待发放/成功/失败台账
- **政策资讯**：发布与浏览资助政策、通知与办理指南，支撑学生端资讯阅读与管理端内容维护
- **管理数据看板**：项目、申请、困难认定与发放等 KPI，以及资助类型、学院分布等 ECharts 运营图表
- **申请评审中台**：院系初审打分与意见、学校终审结论流转，覆盖通过、驳回与进度查询
- **用户与个人中心**：学生资料、学号学院专业、GPA 与困难等级维护，管理员账号启停与角色管理

## 技术架构

- **后端**：Spring Boot 2.7 + MyBatis-Plus + JWT + Lombok
- **前端**：Vue 3 + TypeScript + Vue Router + Pinia + Element Plus + Vite + ECharts
- **数据库**：MySQL 8.0

<!-- screenshots-start -->
## 系统截图

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png" alt="登录页面" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E5%AD%A6%E7%94%9F%E9%A6%96%E9%A1%B5.png" alt="学生首页" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E5%A5%96%E5%8A%A9%E9%A1%B9%E7%9B%AE.png" alt="奖助项目" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E6%88%91%E7%9A%84%E7%94%B3%E8%AF%B7.png" alt="我的申请" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E8%AF%84%E9%80%89%E5%85%AC%E7%A4%BA.png" alt="评选公示" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E8%B5%84%E5%8A%A9%E5%8F%91%E6%94%BE.png" alt="资助发放" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E7%AE%A1%E7%90%86%E5%91%98%E4%BB%AA%E8%A1%A8%E7%9B%98.png" alt="管理员仪表盘" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E7%94%B3%E8%AF%B7%E8%AF%84%E5%AE%A1.png" alt="申请评审" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E8%AE%BA%E6%96%87%E5%9B%BE1.png" alt="论文图1" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/%E8%AE%BA%E6%96%87%E5%9B%BE2.png" alt="论文图2" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/campusscholarship/UML%E5%9B%BE%E5%88%97%E8%A1%A8.png" alt="UML图列表" width="600" />

<!-- screenshots-end -->

---

## 接毕业设计和论文

### 作者微信：vvsgxmn  (支持修改、 部署调试、 支持代做毕设)

### 接网站建设、小程序

### 选题+开题报告+任务书+程序定制+安装调试+论文+答辩ppt 都可以做

### 购买地址：[https://www.vvxx.love](https://www.vvxx.love)（vv毕设网）

### 支持 **一键生成 UML 图**：上传项目压缩包即可自动产出功能模块图、用例图、流程图、E-R 图、时序图等全套毕设图表。

### 提供 **免费配套软件下载 + 安装说明 + 部署教程**

![vv毕设网 - 一键画图](https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/uml-draw.png)

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/image-20260825133349317.png" alt="image-20260825133349317" />

⚠️ Bug添加微信**免费修复**，免费修复。其他平台的私信一律不管（微信方便发送文件）
