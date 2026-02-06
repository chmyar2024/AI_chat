---
# === 核心属性 ===
type: action
mode: quick
status: todo        # todo | doing | done
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/action]

# === 扩展属性 ===
priority: medium    # high/medium/low
due: ""             # YYYY-MM-DD
basis: []           # 依据/理由
counter: []         # 风险/反对因素
project: []         # 执行归属 [[05-Execution/Project]]
<%* if (tp.frontmatter.mode === "deep") { %>
# === Deep Mode 属性 ===
energy_cost: 3      # 1-10
time_estimate: ""   # e.g. 30m
<%* } %>
---

> [!tip] Action: 最小执行单元
> **Quick Mode**: 简单任务清单  
> **Deep Mode**: 包含上下文与预估

---

## ✅ 任务内容

**要做什么**: <%tp.file.cursor(1)%>

**WHY**: [[Compass]] > 

---

## 📋 执行步骤

- [ ] <%tp.file.cursor(3)%>

---

<!-- === DEEP MODE SECTIONS === -->

<%* if (tp.frontmatter.mode === "deep") { %>
---

## ⚡ 上下文 (Deep Mode)

**所需工具/环境**: 
**潜在障碍**: 

### 进度/备注
> 

<%* } %>

---

## 🔗 链接

**项目**: [[05-Execution/Project/]]  
**参考**: [[01-Capture/Clip/]]
