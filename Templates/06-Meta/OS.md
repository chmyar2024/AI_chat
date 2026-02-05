---
# === 核心属性 ===
type: os
mode: deep
status: active
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
updated: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/os]
---

> [!abstract] Personal OS: 个人操作系统
> **用途**: 定义和优化你的个人系统架构  
> **频率**: 每季度更新一次

---

## 🖥️ 系统概览

**版本**: v<%tp.file.cursor(1)%>  
**最后更新**: <%tp.date.now("YYYY-MM-DD")%>  
**状态**: 运行良好 / 需优化 / 重构中

---

## 🏗️ 系统架构

### 核心子系统 (v1.1)
```
Personal OS v1.1
├── 战略层 (Strategy)
│   ├── Compass (价值观+愿景+北极星)
│   ├── Goals (目标管理)
│   └── Principles (原则库)
│
├── 知识层 (Knowledge)
│   ├── Capture (捕获: Signal/Quick/Clip)
│   ├── Process (处理: Insight/System)
│   ├── Tools (思维工具箱) ⭐NEW v1.1
│   ├── Remember (记忆: Recall)
│   ├── Reflect (反思: Loop)
│   └── Map (知识地图)
│
├── 执行层 (Execution)
│   ├── Actions (任务)
│   ├── Projects (项目)
│   └── Creates (创作)
│
├── 网络层 (Network)
│   ├── People (人际)
│   ├── Orgs (组织)
│   ├── Resources (资源)
│   ├── Environment (环境优化) ⭐NEW v1.1
│   └── Vital (生命力管理) ⭐NEW v1.1
│
├── 控制层 (Control)
│   └── Daily (每日调度)
│
└── 元层 (Meta)
    ├── OS (系统文档)
    └── Review (定期复盘)
```

**v1.1 新增模块**:
- 🧰 Tools - 5大思维工具（Scale/Paradox/First Principles/Inversion/Simulation）
- 🏠 Environment - 三维环境优化（物理/数字/社交）
- 💪 Vital - 双底座管理（健康+财务）

---

## ⚙️ 运行规则

### 每日协议
**晨间 (5-10分钟)**:
- [ ] 打开 [[Daily|今日Dashboard]]
- [ ] 查看 Top Priority
- [ ] 复习当日 Recall

**日间 (随时)**:
- [ ] 快速捕获用 [[Signal]]
- [ ] 深度思考用 [[Insight]]

**晚间 (10分钟)**:
- [ ] 清空 Inbox
- [ ] 完成闭环率檢查
- [ ] 设定明日焦点

### 每周协议
- [ ] 周日: 复盘本周 [[Loop]]
- [ ] 周日: 规划下周 Top 3
- [ ] 更新项目进度

### 每月协议
- [ ] 月末: 目标复盘 [[Goal]]
- [ ] 月初: 调整优先级
- [ ] 检查 [[Compass|对齐度]]

### 每季度协议
- [ ] Compass 复审
- [ ] 北极星指标评估
- [ ] 系统优化 (更新此OS文档)

---

## 📊 系统指标

### 健康度监控
| 指标 | 目标 | 当前 | 状态 |
|------|------|------|------|
| Daily 完成率 | >90% | % | 🟢🟡🔴 |
| Inbox 清空率 | 100% | % | 🟢🟡🔴 |
| 项目进展率 | >80% | % | 🟢🟡🔴 |
| 闭环任务率 | >85% | % | 🟢🟡🔴 |
| SRS 复习完成 | >80% | % | 🟢🟡🔴 |

### 效能数据
- **活跃项目数**: (建议 ≤ 5)
- **维护人脉数**: (建议 ≤ 20)
- **⚠️ 需激活人脉**: `$= dv.pages('"03-Network/Person"').where(p => p.status != "archived" && p.relevance >= 7 && (!p.last_contact || (dv.date("today") - dv.date(p.last_contact)).days > 30)).length` 人
- **每周深度思考**: h (建议 ≥ 10h)

---

## 🛠️ 工具栈

### 核心工具
- **PKM**: Obsidian
- **任务**: [[Action|Action System]]
- **日历**: [[Daily|Daily Notes]]
- **间隔复习**: Spaced Repetition Plugin

### 辅助工具
- **剪藏**: [[Clip]]
- **快记**: [[Quick]]
- **查询**: Dataview
- **可视化**: Mermaid

---

## 🔄 系统优化

### 当前问题
1. <%tp.file.cursor(2)%>
2. 

### 改进计划
- [ ] 
- [ ] 

### 实验中的方法
> 

---

## 📚 使用指南

### 新手快速开始
1. 创建 [[Compass]] 确立方向
2. 设置 3 个 [[Goal|目标]]
3. 开始使用 [[Daily]] 每日记录
4. 想法用 [[Signal]] 快速捕获
5. 深度思考用 [[Insight]]

### 模式选择
- **快速模式** (`mode: quick`): 日常使用
- **深度模式** (`mode: deep`): 重要内容

### 救援机制
**系统混乱时**:
1. 停止添加新内容
2. 清空所有 Inbox
3. 复盘最近一周 [[Loop]]
4. 重新对齐 [[Compass]]

---

## 📈 版本历史

### v<%tp.file.cursor(3)%> (<%tp.date.now("YYYY-MM-DD")%>)
- **变更**: 初始化系统
- **优化**: 
- **新增**: 

### 里程碑
- **v1.0**: 系统建立
- **v2.0**: (未来)

---

## 🔗 快速跳转

- [[Daily|📅 今日Dashboard]]
- [[Compass|🧭 价值观愿景]]
- [[Signal|💡 快速捕获]]
- [[Insight|🧠 深度思考]]
- [[Action|✅ 任务管理]]

---

## 💡 设计哲学

> [!quote] 核心理念
> "深度可选，效率优先"
> 
> - 双模式设计让每个人都能找到适合的深度
> - 自动化查询减少手动工作
> - 渐进式复杂度支持长期成长
