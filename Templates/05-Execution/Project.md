---
# === 核心属性 ===
type: project
mode: quick
status: planning    # planning | active | paused | completed
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/project]

# === 扩展属性 ===
priority: medium    # high/medium/low
deadline: ""        # YYYY-MM-DD
basis: []           # 依据/理由
counter: []         # 风险/反对因素
project: [[04-Strategy/Goal]] # 执行对齐/归属
<%* if (tp.frontmatter.mode === "deep") { %>
# === Deep Mode 属性 ===
stakeholders: []
<%* } %>
---

> [!tip] Project: 项目管理
> **Quick Mode**: 任务聚合与进度追踪  
> **Deep Mode**: 战略对齐与复盘

---

## 🎯 目标与成果

**项目名称**: <%tp.file.cursor(1)%>  
**核心目标**: 
> 

---

## ✅ 任务面板

```dataview
TASK FROM "05-Execution/Action"
WHERE project = this.file.link
WHERE !completed
SORT priority DESC, due ASC
```

### 快速添加
- [ ] [[05-Execution/Action/<%tp.file.cursor(2)%>|]]
- [ ] 

---

<!-- === DEEP MODE SECTIONS === -->

<%* if (tp.frontmatter.mode === "deep") { %>
---

## 🧭 战略视角 (Deep Mode)

### 价值验证
**为什么做这个？**: 
**不做会怎样？**: 

### 资源与干系人
**关键干系人**: [[03-Network/Person/]]
**主要资源需求**: 

---

## 🚧 障碍与复盘 (Deep Mode)

### 潜在障碍/风险
- [ ] 风险点1: 应对策略...
- [ ] 风险点2: ...

### 进展/复盘记录
> Start Date: <%tp.date.now("YYYY-MM-DD")%>
> 
> 

<%* } %>

---

## 📊 自动化统计

**完成率**: `$= const tasks = dv.pages('"05-Execution/Action"').where(p => p.project?.path === dv.current().file.path).file.tasks.array(); if(tasks.length === 0) return "0%"; const done = tasks.filter(t => t.completed).length; Math.round((done/tasks.length)*100)`%
