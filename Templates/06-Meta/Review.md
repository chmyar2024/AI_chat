---
# === 核心属性 ===
type: review
mode: deep
status: active
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/review]

# === 扩展属性 ===
period: weekly      # weekly/monthly/quarterly/yearly
date_range: ""      # YYYY-MM-DD - YYYY-MM-DD
related: []
---

> [!abstract] Review: 周期性系统复盘
> **目的**: 保持系统健康，调整航向，清理熵增  
> **频率**: 周/月/季/年

---

## 📅 周期概览

**复盘周期**: `= this.period`  
**时间范围**: `= this.date_range`

---

## 📊 数据回顾 (Data)

### 核心指标
| 指标 | 目标 | 实际 | 状态 |
|------|------|------|------|
| 完成项目 | | | |
| 达成目标 | | | |
| 习惯打卡 | | | |

### 图表视图
```dataview
TABLE status, priority
FROM "05-Execution/Action"
WHERE due >= date(<%tp.file.cursor(1)%>) AND due <= date(<%tp.file.cursor(2)%>)
```

---
> 
> ## 👥 人脉激活清单 (Reconnect)
> 
> ```dataviewjs
> const people = dv.pages('"03-Network/Person"')
>     .where(p => p.status != "archived" && p.relevance >= 7)
>     .where(p => {
>         if (!p.last_contact) return true;
>         const contactDate = dv.date(p.last_contact);
>         if (!contactDate) return true;
>         const days = (dv.date('today') - contactDate).days;
>         return days > 30;
>     })
>     .sort(p => p.relevance, 'desc');
> 
> if (people.length > 0) {
>     dv.table(["Name", "Relevance", "Last Contact", "Days Inactive"],
>         people.map(p => {
>             const last = p.last_contact ? p.last_contact : "Never";
>             let days = "∞";
>             if (p.last_contact) {
>                 const contactDate = dv.date(p.last_contact);
>                 if (contactDate) {
>                    days = Math.floor((dv.date('today') - contactDate).days) + "d";
>                 }
>             }
>             return [p.file.link, p.relevance, last, days];
>         })
>     );
> } else {
>     dv.paragraph("All core relationships are healthy! 🎉");
> }
> ```
> 
> ---

## 🛑 清理与维护 (Cleanup)

- [ ] **Inbox 清空**: (Signal, Quick, Clip)
- [ ] **桌面/下载文件夹清理**
- [ ] **标签整理**: 归档未使用的 tag
- [ ] **项目状态更新**: 归档已完成项目

---

## 🤔 深度反思 (Reflection)

### 本周期最大的胜利
> 

### 本周期最大的阻碍
> 

### Start / Stop / Continue
- **Start (新尝试)**: 
- **Stop (停止做)**: 
- **Continue (保持做)**: 

---

## 🧭 对齐检查 (Alignment)

> [!tip] 检查 Compass
> 对照 [[Compass|指南针]]，确认方向是否偏移

- [ ] 核心价值观是否得到体现？
- [ ] 距离愿景是近了还是远了？
- [ ] 北极星指标进展如何？

---

## 🔮 下一周期规划 (Plan)

### Top 3 目标
1. 
2. 
3. 

### 重点项目
- [[05-Execution/Project/]]
- [[05-Execution/Project/]]

### 预期挑战
- 

---

## 🔗 相关链接

**上一周期**: [[06-Meta/Review/]]  
**相关目标**: [[04-Strategy/Goal/]]  
**相关项目**: [[05-Execution/Project/]]
