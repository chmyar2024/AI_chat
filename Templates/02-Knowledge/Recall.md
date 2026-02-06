---
# === 核心属性 ===
type: recall
claim_type: prompt       # prompt | fact | concept
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
updated: <%tp.date.now("YYYY-MM-DD HH:mm")%>
last_reviewed: ""       # 上次审阅时间 (YYYY-MM-DD)
tags: [neuromancer/recall]

# === 扩展属性 ===
origin_node: ""     # 来源笔记 [[02-Knowledge/Insight]]
review_focus: ""    # 主题驱动复习的焦点
assumptions: []
invalidated_by: []
---

> [!abstract] Recall: 主题驱动复习
> **原则**: 不依赖截止日期，而是围绕主题或问题做回忆  
> **目标**: 强化理解与应用，而非刷题式记忆

---

## 💡 核心内容

### 要记住的是什么？

<%tp.file.cursor(1)%>

---

## 🧠 主动回忆测试

> [!warning] 不要看答案！先尝试回忆

### 问题
**<%tp.file.cursor(2)%>**

---

### 答案 (折叠)
<details>
<summary>点击查看答案</summary>

**正确答案**: 

</details>

---

## 🎯 应用场景

**这个知识点可以用在哪里？**
- 场景1: 
- 场景2: 

**最近一次使用**: 
- 日期: 
- 情况: [[]]

---

## 🔗 知识连接

**来源**: [[02-Knowledge/Insight/<%tp.file.cursor(3)%>]]  
**相关知识**: [[02-Knowledge/System/]]  
**实际应用**: [[05-Execution/Project/]]

---

## 📊 复习记录

**本次复习主题**: `= this.review_focus`  
**上次审阅**: `= this.last_reviewed`

---

## 🎨 记忆增强 (可选)

### 记忆锚点
**视觉锚点**: (简短的图像/场景描述)
> 

**关键词**: #<%tp.file.cursor(4)%> #

---

## ✅ 复习反馈

### 本次复习难度
- ☐ Easy (轻松回忆) → 增加间隔
- ☐ Good (正常) → 保持间隔
- ☐ Hard (困难) → 缩短间隔
- ☐ Again (完全忘记) → 重启R1

### 调整策略
**如果多次 Hard/Again**: 
- [ ] 简化内容
- [ ] 添加更多应用场景
- [ ] 创建记忆锚点
- [ ] 减少一次记忆的信息量

---

## 📈 复习历史

| 日期 | 主题 | 难度 | 备注 |
|------|------|------|------|
| <%tp.date.now("YYYY-MM-DD")%> |  | - | 创建 |
| | | | |

---

## 💡 使用提示

> [!tip] 最佳实践
> 1. 每次复习前先**主动回忆**，不要直接看答案
> 2. 回忆不出来没关系，这正是复习的目的
> 3. 每次复习后记录难度，让系统自动调整间隔
> 4. 如果某个知识点总是忘记，考虑简化或增加应用
