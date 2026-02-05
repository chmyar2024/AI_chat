---
# === 核心属性 ===
type: create
mode: quick  # quick | deep
status: draft
created: <%tp.date.now("YYYY-MM-DD HH:mm")%>
tags: [neuromancer/create]

# === 扩展属性 ===
format: ""          # 文章/视频/课程/产品/设计
audience: ""        # 目标受众
related: []
<%* if (tp.frontmatter.mode === "deep") { %>
# === Deep Mode 属性 ===
impact_goal: ""     # 期望影响
distribution: ""    # 发布渠道
<%* } %>
---

> [!tip] 模板模式
> **Quick Mode** (当前): 简单创作记录  
> **Deep Mode**: 完整创作规划与复盘

---

## 🎨 创作概述

**标题**: <%tp.file.cursor(1)%>

**形式**: `= this.format`  
**受众**: `= this.audience`

---

## 💡 核心想法

**要传达的核心信息**: 
> 

**为什么要创作这个**: 
- 

---

## 📝 内容大纲

### 结构框架
1. <%tp.file.cursor(2)%>
2. 
3. 

---

## ✅ 创作进度

- [ ] 构思
- [ ] 大纲
- [ ] 初稿
- [ ] 修改
- [ ] 定稿
- [ ] 发布

**当前状态**: `= this.status`

---

<!-- === DEEP MODE SECTIONS === -->

<%* if (tp.frontmatter.mode === "deep") { %>
---

## 🎯 目标设定 (Deep Mode)

### 期望影响
**想要达成什么**: `= this.impact_goal`

**成功指标**:
- 阅读量/观看量: 
- 互动率: 
- 转化率: 

### 价值主张
**对受众的价值**: 
- 

**独特性**: (与其他内容的区别)
- 

---

## 📚 知识整合 (Deep Mode)

### 素材来源
- [[02-Knowledge/Insight/]]
- [[02-Knowledge/System/]]
- [[01-Capture/Clip/]]

### 引用资源
1. 
2. 

---

## 🎨 创作策略 (Deep Mode)

### 风格定位
**语气**: (正式/轻松/学术)  
**结构**: (叙事/论述/问答)  
**篇幅**: 

### 吸引元素
- **开头钩子**: 
- **故事案例**: 
- **视觉元素**: 

---

## 📢 发布计划 (Deep Mode)

### 发布渠道
**主要渠道**: `= this.distribution`  
**次要渠道**: 

### 推广策略
- [ ] 社交媒体预热
- [ ] 邮件列表通知
- [ ] 社群分享
- [ ] KOL 推荐

**发布日期**: 

---

## 📊 效果追踪 (Deep Mode)

### 数据监测
| 指标 | 目标 | 实际 | 达成率 |
|------|------|------|--------|
| 阅读/观看 | | | |
| 点赞/分享 | | | |
| 评论互动 | | | |
| 转化行动 | | | |

### 反馈收集
**正面反馈**: 
- 

**改进建议**: 
- 

---

## 🔄 迭代优化 (Deep Mode)

### 复盘总结
**做得好**: 
**可改进**: 
**下次尝试**: 

**提取洞察**: [[02-Knowledge/Insight/<%tp.file.cursor(3)%>|创作方法论]]

<%* } %>

---

## 🔗 相关链接

**支持系统**: [[02-Knowledge/System/]]  
**相关项目**: [[05-Execution/Project/]]  
**目标受众**: [[03-Network/Person/]]

---

## 📎 草稿区

### 随手记录


### 待整理片段

