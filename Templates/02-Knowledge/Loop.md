---
# === 核心属性 ===
type: loop
mode: quick  # quick | deep
status: active
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/loop]

# === 扩展属性 ===
period: daily       # daily/weekly/monthly/project
related: []
up: []              # 关联项目/系统
<%* if (tp.frontmatter.mode === "deep") { %>
# === Deep Mode 属性 ===
impact: medium      # high/medium/low
actionable: true    # 是否有可行动的洞察
<%* } %>
---

> [!tip] 模板模式
> **Quick Mode** (当前): 快速复盘 (3分钟)  
> **Deep Mode**: 深度反思 (15分钟)

---

## 🎯 复盘对象

**类型**: `= this.period`  
**对象**: [[<%tp.file.cursor(1)%>]]

---

## 📊 What - 发生了什么？

### 关键事件
1. 
2. 
3. 

### 结果数据
- **计划**: 
- **实际**: 
- **完成度**: %

---

## 🤔 So What - 意味着什么？

### 做得好的地方
**亮点**: 

**为什么成功**: 

### 需要改进的地方
**问题**: 

**根本原因**: 

---

## 💡 Now What - 下一步怎么做？

### 可行动洞察
- [ ] **继续做**: 
- [ ] **开始做**: 
- [ ] **停止做**: 

---

<!-- === DEEP MODE SECTIONS === -->

<%* if (tp.frontmatter.mode === "deep") { %>
---

## 🏗️ 深度分析 (Deep Mode)

### 五个为什么 (5 Whys)
1. **为什么会这样**? 
2. **为什么会那样**? 
3. **为什么**? 
4. **为什么**? 
5. **根本原因**: 

### 模式识别
**这次和以前类似的情况**: 
- 相似点: 
- 不同点: 

**重复出现的模式**: 
- 

---

## 📈 影响评估 (Deep Mode)

### 直接影响
**对我**: 
**对他人**: 
**对目标**: 

### 长期影响
**3个月后**: 
**1年后**: 

---

## 🎓 提取知识 (Deep Mode)

### 新洞察
**提炼出的原则/规律**: 
> 

**转化为**: [[02-Knowledge/Insight/<%tp.file.cursor(2)%>|创建洞察]]

### 可复用方法
**形成系统**: [[02-Knowledge/System/]]  
**提取原则**: [[04-Strategy/Principle/]]

---

## 🔄 比较分析 (Deep Mode)

| 维度 | 预期 | 实际 | 差异原因 |
|------|------|------|----------|
| 时间 | | | |
| 质量 | | | |
| 资源 | | | |
| 结果 | | | |

<%* } %>

---

## ✅ 行动清单

### 立即行动
- [ ] [[05-Execution/Action/<%tp.file.cursor(3)%>|]]

### 更新文档
- [ ] 更新 [[Compass]] (如影响价值观/愿景)
- [ ] 更新 [[02-Knowledge/System/]] (如发现新模式)

---

## 🔗 相关链接

**关联项目**: [[05-Execution/Project/]]  
**相关系统**: [[02-Knowledge/System/]]  
**产生洞察**: [[02-Knowledge/Insight/]]

---

## 📝 原始记录

### 详细笔记


### 数据/截图


### 参考资料

