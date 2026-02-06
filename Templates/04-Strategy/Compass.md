---
# === 核心属性 ===
type: compass
mode: deep  # Compass 仅支持 deep mode
status: active
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
updated: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/compass]

# === 扩展属性 ===
review_frequency: quarterly  # 复审频率
---

> [!abstract] Compass: 价值观与愿景导航
> **使命**: 我为什么做这些事？  
> **作用**: 所有决策和行动的对齐基准

---

## 🧭 核心价值观 (Values)

### Top 3 价值观
1. **<%tp.file.cursor(1)%>**
   - 定义: 
   - 体现: 

2. ****
   - 定义: 
   - 体现: 

3. ****
   - 定义: 
   - 体现: 

### 价值观冲突
**当X和Y冲突时**: 优先X，因为...

---

## 🎯 愿景 (Vision)

### 3-5年后的理想状态

**生活**: 
> 

**工作**: 
> 

**关系**: 
> 

**成长**: 
> 

### 愿景画面
**闭眼能看到的具体场景**: 
```
<%tp.file.cursor(2)%>
```

---

## 📈 北极星指标 (North Star Metrics)

> [!success] 量化追踪核心目标

```dataviewjs
> const goals = dv.pages('"04-Strategy/Goal"')
>     .where(p => p.status == "active")
>     .sort(p => p.priority, 'desc');
> 
> if (goals.length > 0) {
>     dv.table(["🎯 Goal", "📊 Progress", "📅 Due", "⏳ Days Left"],
>         goals.map(p => {
>             const progress = p.progress || "0%";
>             const progNum = parseInt(progress) || 0;
>             const bar = "▓".repeat(Math.round(progNum/10)) + "░".repeat(10 - Math.round(progNum/10));
>             
>             const due = p.target_date ? dv.date(p.target_date) : null;
>             let daysLeft = "-";
>             if (due) {
>                 const diff = due - dv.date('today');
>                 daysLeft = Math.ceil(diff.days) + "d";
>             }
>             
>             return [
>                 p.file.link,
>                 `${bar} ${progress}`,
>                 due,
>                 daysLeft
>             ];
>         })
>     );
> } else {
>     dv.paragraph("No active goals found. Time to set some!");
> }
> ```

### 指标说明
- **指标1**: 为什么这个指标重要
- **指标2**: 
- **指标3**: 

---

## 🎯 年度聚焦 (Annual Focus)

### <%tp.date.now("YYYY")%> 年主题
**主题**: "<%tp.file.cursor(4)%>"

**三大目标**:
1. [[04-Strategy/Goal/]] - 
2. [[04-Strategy/Goal/]] - 
3. [[04-Strategy/Goal/]] - 

---

## ⚖️ 对齐检查 (Alignment Check)

### 当前项目对齐度

```dataview
TABLE 
  status as "状态",
  progress as "进度",
  choice(
    contains(file.name, "核心关键词"), "🎯 高度对齐",
    "⚠️ 需要评估"
  ) as "对齐度"
FROM "05-Execution/Project"
WHERE status = "active" OR status = "planning"
SORT file.ctime DESC
```

### 对齐问题
**当前正在做但不对齐的事**: 
- 

**应该做但还没做的事**: 
- 

---

## 🔄 决策框架 (Decision Framework)

### 核心问题
在做任何重大决策前问：

1. **对齐测试**: 这个选择让我更接近还是更远离愿景？
2. **价值测试**: 这符合我的核心价值观吗？
3. **北极星测试**: 这会推动我的北极星指标吗？
4. **机会成本**: 说Yes意味着对什么说No？

### 快速决策矩阵
| | 对齐愿景 | 不对齐愿景 |
|---|---|---|
| **高价值** | ✅ 立即做 | ⚠️ 需评估 |
| **低价值** | 🤔 可考虑 | ❌ 拒绝 |

---

## 📅 定期复审 (Regular Review)

### 季度复审 (每3个月)
- [ ] 评估北极星指标进展
- [ ] 检查活跃项目对齐度
- [ ] 更新年度目标状态
- [ ] 调整优先级

### 年度复审 (每年)
- [ ] 愿景是否仍然想要？
- [ ] 价值观是否需要更新？
- [ ] 北极星指标是否需要调整？
- [ ] 设定下一年主题和目标

**下次复审**: <%tp.date.now("YYYY-MM-DD", 90)%>

---

## 📉 进化记录 (Evolution)

### 历史版本

```dataview
LIST FROM "02-Knowledge/Loop"
WHERE type = "loop" AND contains(context, this.file.link)
SORT created DESC
```

### 重大调整
| 日期 | 调整内容 | 原因 |
|------|---------|------|
| <%tp.date.now("YYYY-MM-DD")%> | 建立 Compass | 系统初始化 |
| | | |

---

## 🔗 相关资源

**核心原则**: [[04-Strategy/Principle/]]  
**关键目标**: [[04-Strategy/Goal/]]  
**复盘记录**: [[02-Knowledge/Loop/]]

---

## 💡 灵感与提醒

> [!quote] 座右铭
> "<%tp.file.cursor(5)%>"

### 关键提醒
- 
- 
- 

### 灵感来源
- 人物: [[03-Network/Person/]]
- 书籍: 
- 事件: [[02-Knowledge/Insight/]]
