# Kubernetes 学习仓库

这是一个使用 AI 驱动的个人 Kubernetes 学习仓库，旨在帮助你系统性地掌握 Kubernetes 容器编排技术。

## 仓库简介

本仓库采用 **AI 辅助学习法**，使用 Claude Code 作为交互式导师，帮助你深入理解 Kubernetes 的核心概念和实践技能。

**🚀 新手？** 请查看 [快速开始指南](./GETTING-STARTED.md) 了解如何开始使用本仓库。

## 工作原理

这个仓库使用 Claude Code 作为交互式 Kubernetes 导师，特点包括：
- 使用苏格拉底式教学法（先了解你已掌握的内容）
- 提供简洁明了的解释（约 200 字）
- 通过后续问题验证你的理解
- 根据你的反馈调整教学风格
- 追踪每次学习会话，个性化你的学习体验

## 仓库结构

```
/sessions/                    # 日常学习会话记录
  /2026-01-20/               # 按日期组织的学习记录
  /2026-01-21/
  SESSION-TEMPLATE.md        # 会话记录模板

/progress/                    # 学习进度的单一真相来源
  k8s-study-tracker.md       # 综合进度追踪器，包括：
                             # - 所有 K8s 主题映射
                             # - 已掌握的主题
                             # - 识别出的知识盲区
                             # - 学习计划

CLAUDE.md                     # AI 导师指令（苏格拉底式教学法）
README.md                     # 本文件
```

## 使用方法

### 日常学习会话

1. 在此仓库中打开 Claude Code
2. 像与导师交谈一样自然地提出关于 Kubernetes 的问题
3. 回答 Claude 提出的理解检查问题
4. 每次会话后，Claude 会自动记录：
   - 你学到的内容
   - 你遇到困难的地方
   - 你已掌握的内容
   - 下一步需要复习的内容

### 复习会话

当你想要复习时，可以简单地问 Claude：
- "让我们复习一下我遇到困难的主题"
- "今天我应该专注学习什么？"
- "在我的薄弱领域测试我"
- "显示我的学习进度"

Claude 会读取你的会话历史，并基于你过去的表现创建个性化的复习内容。

### 追踪你的进度

查看 `/progress/k8s-study-tracker.md` 的综合学习追踪器，了解：
- 整体学习准备情况
- 已完成的主题领域
- 剩余的知识盲区
- 优先学习计划

## 学习理念

**引导式学习方法：**
- 对话式且无评判性
- 基于你现有的知识构建
- 在继续前进之前检查理解
- 适应你的学习风格
- 专注于深入理解，而非死记硬背

## Kubernetes 学习主题

本仓库覆盖以下 Kubernetes 核心主题：

### 1. Kubernetes 基础 (15%)
- K8s 架构和组件概览
- 核心概念：集群、节点、Pod
- kubectl 基础命令
- YAML 配置基础

### 2. 工作负载管理 (20%)
- Pods 生命周期和管理
- Deployments
- StatefulSets
- DaemonSets
- Jobs 和 CronJobs
- ReplicaSets

### 3. 服务和网络 (15%)
- Services（ClusterIP、NodePort、LoadBalancer）
- Ingress 和 Ingress Controllers
- Network Policies
- DNS 和服务发现
- 负载均衡

### 4. 配置和存储 (15%)
- ConfigMaps
- Secrets
- Persistent Volumes (PV)
- Persistent Volume Claims (PVC)
- Storage Classes
- Volume 类型

### 5. 安全性 (10%)
- RBAC（Role-Based Access Control）
- Service Accounts
- Security Contexts
- Pod Security Policies/Standards
- Network Policies

### 6. 调度和资源管理 (10%)
- 资源请求和限制
- Node Selectors 和 Affinity
- Taints 和 Tolerations
- 自动扩展（HPA、VPA）
- LimitRanges 和 ResourceQuotas

### 7. 监控和故障排查 (10%)
- 日志管理
- 监控指标
- 健康检查（Liveness、Readiness、Startup Probes）
- 常见问题排查
- kubectl 调试技巧

### 8. 高级主题 (5%)
- Helm 包管理
- Operators
- Custom Resource Definitions (CRDs)
- 多集群管理
- GitOps 实践

## 学习资源

### 官方资源
- [Kubernetes 官方文档](https://kubernetes.io/docs/)
- [Kubernetes GitHub](https://github.com/kubernetes/kubernetes)
- [CNCF 云原生互动景观](https://landscape.cncf.io/)

### 实践环境
- [Minikube](https://minikube.sigs.k8s.io/) - 本地 K8s 集群
- [Kind](https://kind.sigs.k8s.io/) - Docker 中的 K8s
- [K3s](https://k3s.io/) - 轻量级 K8s
- [Play with Kubernetes](https://labs.play-with-k8s.com/) - 在线练习环境

### 认证考试
- [CKA (Certified Kubernetes Administrator)](https://www.cncf.io/certification/cka/)
- [CKAD (Certified Kubernetes Application Developer)](https://www.cncf.io/certification/ckad/)
- [CKS (Certified Kubernetes Security Specialist)](https://www.cncf.io/certification/cks/)

## 关键特性

**个性化学习**：
- 详细记录的学习会话和笔记
- 苏格拉底式教学法（基于你已知的内容构建）
- 基于你的反馈的自适应解释
- 针对薄弱领域的定制练习

**全面追踪**：
- 每个会话自动记录
- 识别并追踪知识盲区
- 标记已掌握主题的信心水平
- 根据学习目标衡量进度

**基于证据的方法**：
- 所有答案都经过权威来源验证（Kubernetes 官方文档、CNCF）
- 对技术问题不做猜测
- 为复杂规则提供引用
- 专注于理解"为什么"而不仅仅是"是什么"

## 如何使用此仓库进行 Kubernetes 学习

1. **克隆此仓库**：
   ```bash
   git clone https://github.com/yourusername/ailearn-k8s.git
   cd ailearn-k8s
   ```

2. **清除示例历史**（可选，如果你想从头开始）：
   ```bash
   rm -rf progress/ sessions/
   ```

3. **运行 Claude Code**：
   ```bash
   claude-code
   ```

4. **开始学习！** 开始提出 Kubernetes 问题，Claude 将：
   - 使用苏格拉底式教学法教导你
   - 自动创建 `progress/` 和 `sessions/` 文件夹
   - 追踪你的学习旅程
   - 适应你的学习风格

`CLAUDE.md` 文件包含了 Claude 如何辅导你的所有指令。**它神奇地工作！**

## 开始学习

只需启动与 Claude Code 的对话，提出你的第一个 Kubernetes 问题。Claude 将引导你从那里开始，同时自动追踪你的进度。

示例问题：
- "什么是 Kubernetes Pod？"
- "Deployment 和 StatefulSet 有什么区别？"
- "如何在 K8s 中配置持久化存储？"
- "解释一下 K8s 的网络模型"

---

## 致谢

本仓库的学习框架设计灵感来自 [chenran818/CFP-study](https://github.com/chenran818/CFP-study)。感谢作者分享了如何使用 Claude Code 和 AI 辅助学习方法来系统性地掌握复杂知识领域的优秀实践。

他使用这种 AI 驱动的学习方法成功通过了 CFP（Certified Financial Planner）考试，这证明了这种学习框架的有效性。我们将同样的方法应用于 Kubernetes 学习，希望能帮助更多人掌握云原生技术。

## 贡献

欢迎提交 Issue 和 Pull Request 来改进这个学习框架！

## 许可证

MIT License

---

使用 AI 驱动的学习方法，系统性地掌握 Kubernetes！
