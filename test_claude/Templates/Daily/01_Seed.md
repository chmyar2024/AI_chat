---
# === Layer 1: 核心必需属性 (ALL) ===
type: seed
status: inbox
created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
updated: <% tp.date.now("YYYY-MM-DD HH:mm") %>
summary: ""
aliases: []
tags:
  - neuromancer/seed

# === Layer 2: 通用可选属性 ===
value: medium             # 评估度量: low/medium/high/critical
energy_type: rational     # 能量类型: rational/creative/emotional/physical
categories: []            # 分类组织: 按需填写

# === Layer 3: 特殊属性 (Seed专属) ===
source: ""                # 来源: URL/书籍/对话
format: idea              # 格式: idea/article/conversation/image
---

> [!NOTE] 核心原则
> **目的**: 捕捉任何有价值输入，不分类焦虑
> **触发**: 任何引起你注意的信息/想法/人/经历
> **规则**: 30秒内完成记录，不追求完美

> [!TIP] Seed vs Intuition 边界
> **用Seed**: 如果能说清楚来源（文章/对话/观察/事件）
> **用Intuition**: 如果是"莫名的感觉/预感/内在信号"
> - Seed = 外部信号（可追溯来源）
> - Intuition = 内部信号（无法解释为什么知道）


## 🎯 原始记录
用最原始的语言记录，不加修饰：
"{{原始内容或感受}}"

## 🤔 直觉反应
第一感觉是什么？(不要分析)
- 兴奋？困惑？抗拒？好奇？
- 为什么这个引起了我的注意？

## 🔗 快速连接
这个与我已有的什么相关？(最多3个)
- [[06_Insight/XXX]]
- [[07_System/YYY]]
- [[02_Action/ZZZ]]

## ⏸️ 下一步
- [ ] 立即深入: → 创建 Insight
- [ ] 稍后处理: 设置提醒 <% tp.date.now("YYYY-MM-DD", 3) %>
- [ ] 暂时搁置: 归档，信任未来自己

# 如果是实体，额外记录
## 🏢 实体详情 (仅当format为person/tool/organization时)
- **核心价值**: 这个实体可以为我提供什么？
- **我的价值**: 我可以为这个实体提供什么？
- **关系状态**: 当前关系如何？如何维护？
- **下一步**: 具体什么时间，通过什么方式联系/使用？

--- 
**处理时间目标**: < 5分钟
**转化率要求**: 每周至少将3个Seed转化为Insight或Action
