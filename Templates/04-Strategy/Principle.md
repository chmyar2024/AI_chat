---
# === 核心属性 ===
type: principle
maturity: stable     # developing | stable | evergreen
claim_type: principle # principle | heuristic
confidence: 0.7
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
updated: <%tp.date.now("YYYY-MM-DD HH:mm")%>
last_reviewed: ""    # 上次审阅时间 (YYYY-MM-DD)
tags: [neuromancer/principle]

# === 扩展属性 ===
domain: ""          # 适用领域
origin_link: ""     # 外部来源
origin_node: ""     # 内部来源
basis: []
counter: []
project: [[04-Strategy/Compass]]
assumptions: []
invalidated_by: []
supersedes: []
---

> [!abstract] Principle: 行为原则/决策规则
> **用途**: 提炼可复用的行为原则和决策规则  
> **触发**: 发现有效的决策模式或行为准则

---

## 🎯 原则声明

**原则名称**: <%tp.file.cursor(1)%>

**核心表述**: 
> "在 [场景] 下，我会 [行为]，因为 [原因]"

---

## 📖 详细说明

### 适用场景
**什么时候用**: 
- 

**不适用场景**: 
- 

---

## 💡 原则来源

**外部来源**: `= this.origin_link`  
**内部来源**: `= this.origin_node`  
**提炼自**: [[02-Knowledge/Insight/]]  
**验证于**: [[02-Knowledge/Loop/]]

---

## 🎯 实践指南

### 具体做法
1. <%tp.file.cursor(2)%>
2. 
3. 

### 示例
**情况A**: 
- **应用**: 
- **结果**: 

**情况B**: 
- **应用**: 
- **结果**: 

---

## ⚖️ 权衡取舍

### 带来的好处
- 

### 可能的代价
- 

### 冲突处理
**当与X原则冲突时**: 
> 

---

## 📈 使用记录

```dataview
LIST FROM "00-Core" OR "02-Knowledge/Loop"
WHERE contains(file.outlinks, this.file.link)
SORT file.ctime DESC
LIMIT 10
```

### 效果追踪
| 日期 | 场景 | 应用效果 | 调整 |
|------|------|---------|------|
| <%tp.date.now("YYYY-MM-DD")%> | | | |

---

## 🔄 原则演化

### 版本历史
**v1.0** (<%tp.date.now("YYYY-MM-DD")%>): 初始版本  
**调整原因**: 

---

## 🔗 相关链接

**对齐**: [[Compass|价值观]]  
**来源洞察**: [[02-Knowledge/Insight/]]  
**应用项目**: [[05-Execution/Project/]]

---

## 💡 提醒

> [!warning] 检查点
> 在 [特定场景] 前，记得应用此原则
