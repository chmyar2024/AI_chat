---
# === 核心属性 ===
type: person
mode: quick
status: active      # active | archived (关注度)
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/person]

# === 扩展属性 ===
relevance: 5        # 关联紧密度 (1-10) - 邓巴数权重
last_contact: ""    # YYYY-MM-DD
related: []
up: []              # 所属组织 [[03-Network/Org]]
---

> [!tip] Person: 关系节点
> **Quick Mode**: 价值交换与基本信息  
> **Deep Mode**: 深度关系维护

---

## 👤 基本画像

**姓名**: <%tp.file.cursor(1)%>  
**角色**: <%tp.file.cursor(2)%>  

---

## 🤝 价值交换 (Value)

**对方能提供 (Value In)**: 
- 

**我能提供 (Value Out)**: 
- 

**共识/共同目标**: 
- 

---

## 📅 互动审计

```dataview
LIST FROM "00-Core" OR "05-Execution"
WHERE contains(file.outlinks, this.file.link)
SORT file.ctime DESC
LIMIT 5
```

---

<!-- === DEEP MODE SECTIONS === -->

<%* if (tp.frontmatter.mode === "deep") { %>
---

## ❤️ 关系动态 (Deep Mode)

### 关系深度
**温度 (1-10)**: `= this.relevance`
- 1-3: 弱连接 (需定期清理)
- 4-7: 强连接 (定期维护)
- 8-10: 核心圈 (深度投入)

### 互动记录
> 在这里自由记录关键的互动感受、信任变化或重要时刻...
> 
> 

---

## 🔄 维护策略 (Deep Mode)

**联系频率**: 
**话题/切入点**: 
**下一步计划**: 

<%* } %>

---

## ⚠️ 熵增预警

> [!info] 邓巴数检查
> **Last Contact**: `= this.last_contact`
> **Action**: 如果长期无互动且 Relevance < 3 -> 考虑 Archive
