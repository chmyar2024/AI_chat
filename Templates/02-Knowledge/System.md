---
# === 核心属性 ===
type: system
claim_type: model         # model | framework | theory
maturity: developing    # developing | stable | evergreen
confidence: 0.6
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
updated: <%tp.date.now("YYYY-MM-DD HH:mm")%>
last_reviewed: ""       # 上次审阅时间 (YYYY-MM-DD)
tags: [neuromancer/system]

# === 扩展属性 ===
domain: ""          # 领域 (技术/商业/生活)
basis: []
counter: []
assumptions: []
invalidated_by: []
supersedes: []
---

> [!tip] System: 知识结构与模型
> **默认深度**: 建议写清系统边界与关键假设  
> **控制负担**: 先写核心要素，细化可延后

---

## 🎯 系统定义

**名称**: <%tp.file.cursor(1)%>  
**一句话描述**: 
> 

**适用领域**: `= this.domain`

---

## 🧩 核心要素

### 主要组件
1. **<%tp.file.cursor(2)%>**
2. 
3. 

### 运作机制
**输入** → **处理** → **输出**

---

## 🔍 证据与边界 (Epistemic)

**关键假设**:
- 

**适用边界**:
- 

**失效条件**:
- 

---

## 📚 核心洞察

```dataview
LIST FROM "02-Knowledge/Insight"
WHERE contains(context, this.file.link) OR contains(basis, this.file.link)
SORT maturity DESC
```

---

## 🏗️ 架构与原理 (可选)

### 底层逻辑
**核心原理**: 

**关键假设**: 
- 

### 系统边界
**适用场景**: 
**失效场景**: 

---

## 🔗 系统连接 (可选)

**上游依赖**: [[02-Knowledge/System/]]  
**下游应用**: [[02-Knowledge/System/]]  
**相关模型**: [[02-Knowledge/System/]]

---

## 🎓 学习资源 (可选)

- 核心书籍: 
- 关键论文/文章: 
- 实践案例: [[05-Execution/Project/]]

---

## 🧠 记忆索引

**关键词**: #<%tp.file.cursor(3)%> #

---

## 🧬 版本演化 (Lifecycle)

**变更记录**:
- v1.0 (<%tp.date.now("YYYY-MM-DD")%>): 初始版本
- 
