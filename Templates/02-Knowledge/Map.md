---
# === 核心属性 ===
type: map
mode: quick
status: active
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/map]

# === 扩展属性 ===
domain: ""          # 知识领域
---

> [!abstract] Map of Content (MOC)
> **定义**: 知识的港口与中转站  
> **作用**: 聚合特定主题下的笔记，提供导航视图  
> **区别**: 比 System 轻，不追求建模，只追求聚合

---

## 🗺️ 导航视图

**主题**: <%tp.file.cursor(1)%>

### 🔑 核心概念 (Key Concepts)
- [[02-Knowledge/Insight/]] - (一句话描述)
- [[02-Knowledge/Insight/]]
- 

### 🏗️ 结构/流程 (Structure)
1. [[02-Knowledge/Insight/]]
   - 子概念: [[02-Knowledge/Insight/]]
2. [[02-Knowledge/Insight/]]

---

## 📥 待整理 (Inbox)

> [!info] 自动聚合相关笔记
> ```dataview
> LIST FROM "02-Knowledge"
> WHERE (contains(up, this.file.link) OR contains(tags, this.file.name)) AND file.name != this.file.name
> SORT maturity DESC
> ```

---

## 🚀 相关项目

- [[05-Execution/Project/]]
