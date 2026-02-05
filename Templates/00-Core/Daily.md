---
type: "[[Daily]]"
mode: quick
status: active
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags:
  - neuromancer/daily
energy_level: 5
---

> [!tip] Daily Dashboard
> **Quick Mode**: 3分钟晨间引导  
> **Deep Mode**: 完整日间复盘

---

## 🎯 意图对齐 (Focus)

**今日 One Thing**: [[<%tp.file.cursor(1)%>]]  
**对齐 Compass**: 

---

## ⚡ 执行面板 (Action)

> [!todo] 自动适配任务 (Energy Matches)
> ```dataviewjs
> const energy = dv.current().energy_level || 5;
> const pages = dv.pages('"05-Execution/Action"')
>     .where(p => p.status != "done" && p.status != "archived")
>     .where(p => (p.energy_cost || 5) <= energy)
>     .sort(p => p.priority, 'desc');
> 
> const tasks = pages.file.tasks.where(t => !t.completed);
> 
> if (tasks.length > 0) {
>     dv.taskList(tasks.limit(10));
> } else {
>     dv.paragraph(`> [!info] 当前能量(${energy})下无匹配任务，好好休息！`);
> }
> ```

---

## 📝 快速捕获 (Inbox)

### 💡 想法与待办
- <%tp.file.cursor(3)%>
- [ ] 

---

## 🌙 晚间闭环 (Review)

**闭环率**: `$= const tasks = dv.current()?.file?.tasks; if(!tasks) return "0%"; const done = tasks.filter(t => t.completed).length; Math.round((done/tasks.length)*100) || 0`%

**明日启动**: 明天第一件事做什么？
> 

---

<!-- === DEEP MODE SECTIONS === -->

<%* if (tp.frontmatter.mode === "deep") { %>
---

## 📊 能量与状态 (Deep Mode)

### 能量管理
**今日能量预算**: (1-10)
- [ ] 保护**高能时段**用于 [[Project|深度工作]]
- [ ] 低能时段处理杂事

### 状态自检
- **睡眠**: <%tp.file.cursor(4)%>h
- **运动**: 
- **心情**: 

---

## � 深度复盘 (Deep Mode)

### 满意度检查
- **亮点 (High)**: 
- **低谷 (Low)**: 

### 记忆训练
**今日复习任务**:
```dataview
LIST FROM "02-Knowledge/Recall"
WHERE sr-due = date(today)
LIMIT 3
```

<%* } %>

---

## ⚡ 快速跳转
- [[Signal|💡 捕获]]
- [[Action|✅ 任务]]
- [[Compass|🧭 愿景]]
- [[Insight|� 思考]]

---

## � 时间流
```dataview
LIST FROM ""
WHERE created >= date(today) AND created < date(tomorrow)
SORT file.ctime DESC
```
