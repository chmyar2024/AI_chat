---
# === 核心属性 ===
type: goal
mode: quick  # quick | deep
status: active
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/goal]

# === 扩展属性 ===
target_date: ""     # 目标完成日期
progress: 0%
priority: high      # high/medium/low
related: []
up: [[04-Strategy/Compass]]  # 对齐 Compass
<%* if (tp.frontmatter.mode === "deep") { %>
# === Deep Mode 属性 ===
category: ""        # 生活/工作/健康/财务/关系/成长
measurement: ""     # 衡量标准
<%* } %>
---

> [!tip] 模板模式
> **Quick Mode** (当前): OKR快速追踪  
> **Deep Mode**: 完整目标管理与分解

---

## 🎯 目标定义

**目标**: <%tp.file.cursor(1)%>

**SMART检查**:
- ☐ **S**pecific (具体)
- ☐ **M**easurable (可衡量)
- ☐ **A**chievable (可达成)
- ☐ **R**elevant (相关性)
- ☐ **T**ime-bound (有期限)

---

## 📊 OKR 框架

### Objective (目标)
**我想达成什么**: 
> 

### Key Results (关键结果)
1. **KR1**: <%tp.file.cursor(2)%>
   - 当前: 
   - 目标: 
   - 进度: ☐☐☐☐☐

2. **KR2**: 
   - 当前: 
   - 目标: 
   - 进度: ☐☐☐☐☐

3. **KR3**: 
   - 当前: 
   - 目标: 
   - 进度: ☐☐☐☐☐

---

## ✅ 关键行动

```dataview
TASK FROM "05-Execution/Action"
WHERE up = this.file.link
WHERE !completed
SORT priority DESC
```

### 快速添加
- [ ] [[05-Execution/Action/]]
- [ ] 

---

<!-- === DEEP MODE SECTIONS === -->

<%* if (tp.frontmatter.mode === "deep") { %>
---

## 🧭 战略对齐 (Deep Mode)

### Compass 对齐
**对齐价值观**: [[Compass]] > 
**对齐愿景**: 
**对齐北极星指标**: 

### 为什么这个目标重要？
**内在动机**: 
**外在价值**: 

---

## 🗺️ 路径规划 (Deep Mode)

### 里程碑分解
| 里程碑 | 目标日期 | 状态 | 产出 |
|--------|---------|------|------|
| M1: <%tp.file.cursor(3)%> | | ⏳ | |
| M2:  | | ⏳ | |
| M3:  | | ⏳ | |

### 资源需求
**时间投入**: 
**资金预算**: 
**知识准备**: [[02-Knowledge/System/]]
**人脉支持**: [[03-Network/Person/]]

---

## 🚧 障碍与风险 (Deep Mode)

### 已知障碍
1. **障碍**: 
   - **应对**: 

2. **障碍**: 
   - **应对**: 

### 风险管理
| 风险 | 概率 | 影响 | 缓解措施 |
|------|------|------|----------|
| | 高/中/低 | 高/中/低 | |

---

## 📈 进度追踪 (Deep Mode)

### 周度更新

**<%tp.date.now("YYYY-MM-DD")%>**
- **完成**: 
- **进行中**: 
- **阻塞**: 
- **下周计划**: 

### 月度复盘
| 月份 | KR1进展 | KR2进展 | KR3进展 | 整体评分 |
|------|---------|---------|---------|----------|
| <%tp.date.now("YYYY-MM")%> | % | % | % | /10 |

<%* } %>

---

## 🎯 当前状态

**整体进度**: `= this.progress`  
**截止日期**: `= this.target_date`  
**优先级**: `= this.priority`

---

## 🔄 快速检查

### 每周问题
1. 本周为这个目标做了什么？
2. 是否在正轨上？
3. 需要调整吗？

### 调整触发
- [ ] 进度落后 > 20%
- [ ] 外部环境变化
- [ ] 优先级调整
- [ ] 资源不足

---

## 🔗 相关资源

**支撑项目**: [[05-Execution/Project/]]  
**相关洞察**: [[02-Knowledge/Insight/]]  
**学习资源**: [[02-Knowledge/System/]]

---

## 📊 自动化视图

### 关联任务
```dataview
TABLE 
  status as "状态",
  priority as "优先级",
  due as "截止"
FROM "05-Execution/Action"
WHERE up = this.file.link
SORT status ASC, priority DESC
```

### 完成率
`$= const tasks = dv.pages('"05-Execution/Action"').where(p => p.up?.path === dv.current().file.path).file.tasks.array(); if(tasks.length === 0) return "0%"; const done = tasks.filter(t => t.completed).length; Math.round((done/tasks.length)*100)`%
