---
# === 核心属性 ===
type: system
mode: quick
maturity: developing    # developing | stable | evergreen
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/system]

# === 扩展属性 ===
domain: ""          # 领域 (技术/商业/生活)
related: []
<%* if (tp.frontmatter.mode === "deep") { %>
# === Deep Mode 属性 ===
complexity: medium  # complexity level
<%* } %>
---

> [!tip] System: 知识结构与模型
> **Quick Mode**: 快速定义系统边界  
> **Deep Mode**: 深度系统建模

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

## 📚 核心洞察

```dataview
LIST FROM "02-Knowledge/Insight"
WHERE up = this.file.link OR contains(related, this.file.link)
SORT maturity DESC
```

---

<!-- === DEEP MODE SECTIONS === -->

<%* if (tp.frontmatter.mode === "deep") { %>
---

## 🏗️ 架构与原理 (Deep Mode)

### 底层逻辑
**核心原理**: 

**关键假设**: 
- 

### 系统边界
**适用场景**: 
**失效场景**: 

---

## 🔗 系统连接 (Deep Mode)

**上游依赖**: [[02-Knowledge/System/]]  
**下游应用**: [[02-Knowledge/System/]]  
**相关模型**: [[02-Knowledge/System/]]

---

## 🎓 学习资源 (Deep Mode)

- 核心书籍: 
- 关键论文/文章: 
- 实践案例: [[05-Execution/Project/]]

<%* } %>

---

## 🧠 记忆索引

**关键词**: #<%tp.file.cursor(3)%> #
