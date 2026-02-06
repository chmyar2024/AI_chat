---
# === 核心属性 ===
type: insight
claim_type: hypothesis   # observation | hypothesis | model | principle
maturity: budding       # budding | validating | mature | internalized
confidence: 0.6         # 0-1, epistemic confidence
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
updated: <%tp.date.now("YYYY-MM-DD HH:mm")%>
last_reviewed: ""       # 上次审阅时间 (YYYY-MM-DD)
tags: [neuromancer/insight]

# === 扩展属性 ===
context: []         # 语境/MOC [[02-Knowledge/Map]]
basis: []           # 依据/支撑
counter: []         # 反对观点/竞争假说 (关键新增)
assumptions: []     # 关键假设
invalidated_by: []  # 被哪些证据/洞察推翻
supersedes: []      # 替代哪些旧洞察
---

> [!tip] 记录原则
> **默认深度**: 以清晰命题 + 辩证结构为主  
> **控制负担**: 2分钟内写完核心区块即可

---

## 💡 核心命题 (Thesis)

**Atomic Idea**: <%tp.file.cursor(1)%>

> [!success] 结构化陈述
> **Context (语境)**: 在...情况下
> **Signal (信号)**: 观察到...
> **Insight (洞察)**: 我认为...因为...

---

## 🌉 上下文挂钩 (Context Hooks)

**这个洞察反驳了什么？** (Anti-Pattern)
- 此前我/主要观点认为...，但其实...

**这个洞察解释了什么？** (Explanation)
- 它解释了为什么...现象会发生

---

## 🔍 证据与可信度 (Epistemic)

**证据类型**: (观察/实验/二手资料/推理)

**关键依据**:
1. 
2. 

**不确定性来源**:
- 

---

## 🛠️ 应用实验室

**如果这是真的，那意味着...**:
1. 
2. 

**验证案例**: [[<%tp.file.cursor(2)%>]]

---

## ⚖️ 深度辩证 (可选)

### 竞争假说 (Competing Hypotheses)
**其他可能的解释**:
- 假说A: ...
- 假说B: ...

**为什么本洞察更好**:
- 因为...

### 边界测试 (Boundary Check)
**失效场景**: 
- 当 [变量] 改变时，此结论失效。

---

## 🧠 认知内化 (可选)
> 
### 决策实验 (Decision Application)
> [!important] 反向压力测试
> 在标记为 `internalized` 之前，必须至少完成 3 次决策应用验证，或转化为原则。

**应用尝试**:
1. 
2. 
3. 

### 内化检查 (Status Check)
```dataviewjs
const currentPath = dv.current().file.link;
const loops = dv.pages('"02-Knowledge/Loop"').where(p => p.file.outlinks.includes(currentPath)).length;
const principles = dv.pages('"04-Strategy/Principle"').where(p => p.file.outlinks.includes(currentPath)).length;

const isReady = loops >= 3 || principles >= 1;
const color = isReady ? "green" : "orange";
const icon = isReady ? "✅" : "🚧";

dv.paragraph(`**State**: <span style="color:${color}">${icon} ${isReady ? "Ready for Internalization" : "Validation Needed"}</span>`);
dv.paragraph(`- **Loop Verifications**: ${loops} / 3`);
dv.paragraph(`- **Principle Extractions**: ${principles} / 1`);
```

**记忆锚点**: <%tp.file.cursor(3)%>

**费曼技巧**:
> 试着用最简单的语言（不带术语）向一个12岁孩子解释：
> 
> 

---

## 🧬 版本演化 (Lifecycle)

**变更记录**:
- v1.0 (<%tp.date.now("YYYY-MM-DD")%>): 初始命题
- 

---

## 🔄 链接网络

**MOC (地图)**: [[02-Knowledge/Map/]]  
**来源 (Origin)**: [[01-Capture/Clip/]]  
**反向链接 (Counter)**: [[02-Knowledge/Insight/]]  

---

## 📊 引用此处的笔记
```dataview
LIST FROM [[]]
WHERE file.name != this.file.name
```
