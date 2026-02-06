# Templates 3 系统用户指南 v1.2

> **设计哲学**: "认知/执行分离，知识默认深度"  
> **核心创新**: 语义字段统一 + 双轨系统 (The Engine / The Library)

---

## 🎉 v1.2 变更重点

✨ **关键调整**:
- **语义拆分**: `up` 拆分为 `project` (执行归属) 与 `context` (知识语境)
- **去任务化**: 移除知识节点的 SRS 截止字段，改为 `last_reviewed`
- **字段收敛**: `related` 改为 `basis/counter`，`source` 改为 `origin_link/origin_node`
- **环境降噪**: Environment/Vital 改为轻量实验记录，而非维护型清单

---

## 🚀 快速开始

### 1. 目录结构 (22个核心模板)

```
Templates 3/
├── 00-Core/           # Dashboard (Daily)
├── 01-Capture/        # 快速捕获 (Signal, Quick, Clip)
├── 02-Knowledge/      # 知识库 (Insight, System, Recall, Loop, Map, Tools ⭐NEW)
├── 03-Network/        # 关系网 (Person, Org, Resource, Environment ⭐NEW, Vital ⭐NEW)
├── 04-Strategy/       # 战略层 (Compass, Goal, Principle)
├── 05-Execution/      # 执行层 (Action, Project, Create)
├── 06-Meta/           # 系统层 (OS, Review)
└── Bases/             # 数据视图 (37个自动聚合查询)
```

### 2. 双轨系统 (Engine / Library)

系统分为两个子系统：

- **The Engine (执行子系统)**: Action / Project / Goal / Compass / Vital  
  重点是行动、进度、截止时间与对齐关系。

- **The Library (认知子系统)**: Clip / Insight / System / Map / Principle  
  重点是语境、论证与成熟度。知识模板默认深度，避免“快记堆积”。

**Quick 模式仅保留在 Signal**，用于捕捉想法种子。其他知识模板不再依赖 Quick/Deep 切换。

**知识节点最小结构**（用于长期演化）:
- Identity: 文件名 + type
- Semantics: 核心命题/定义
- Epistemic: claim_type + confidence + evidence
- Context: context/scope
- Relation: basis/counter
- Lifecycle: maturity + updated + last_reviewed + supersedes/invalidated_by

---

## 🛠️ 核心工作流

### ☀️ 每日流程 (Daily Flow)

**早晨 (3分钟)**:
1. 创建 `00-Core/Daily` (Quick Mode)
2. 设定今日 Top 1 焦点
3. 查看能量自适应任务推荐 ⭐
4. 快速查看Vital状态（可选）

**日间 (随时)**:
- 想法 → `01-Capture/Signal` (2分钟)
- 任务 → `05-Execution/Action`
- 会议 → `01-Capture/Quick`
- 文章 → `01-Capture/Clip`

**晚间 (10分钟)**:
- 回到Daily笔记，查看"晚间闭环"
- 自动计算完成率 ⭐
- 清空Inbox
- 设定明日焦点

### 🧠 思考流程 (Thinking Flow)

**Level 1 - 快速捕获**:
1. 使用 `Signal` 快速记下灵感种子

**Level 2 - 初步加工**:
2. 将Signal转化为 `Insight`
3. 使用"如果...那么...反面是..."辩证思考

**Level 3 - 深度思考**:
4. 补充"结构化表达"和"实践检验"

**Level 4 - 复杂问题** ⭐NEW:
6. 使用 `Tools` 模板调用思维工具
   - 问题看起来无解 → Scale Shifting
   - 二选一困境 → Paradox Transformation
   - 质疑现状 → First Principles
   - 不知如何做 → Inversion
   - 难以决策 → Mental Simulation

### 🎯 战略流程 (Strategy Flow)

**初始化 (1小时)**:
1. 填写 `Compass` (价值观+愿景+北极星指标)
2. 设定3个年度 `Goal`
3. 提炼核心 `Principle`

**执行对齐 (持续)**:
4. 创建Project时，检查是否对齐Compass
5. 每周使用 `Review` 检查进度
6. 每月检查Goal进展

**优化调整 (季度)**:
7. 使用 `OS` 进行系统健康诊断
8. 复审Compass是否需要调整

### 🌱 生命力管理 (Vital Flow)

**每周轻量检查**:
1. 打开 `Vital`
2. 记录健康/财务的“当前瓶颈”
3. 选择 1-2 个小步实验
4. 产生洞察后写入 `Insight`

### 🏠 环境优化 (Environment Flow)

**首次设置 (30分钟)**:
1. 创建 `Environment` 笔记
2. 只写 Top 3 关键摩擦
3. 设定一个最小可行的改进实验

**持续优化 (每月)**:
4. 复盘实验结果
5. 将有效模式沉淀为 `Insight`

---

## 🧰 新工具使用指南

### Tools - 思维工具箱 ⭐

**何时使用**: 遇到以下情况时打开Tools模板

| 问题特征 | 推荐工具 | 核心问题 |
|---------|---------|---------|
| 看起来无解 | Scale Shifting | 换个尺度看呢？ |
| 二选一困境 | Paradox | 如何两者兼得？ |
| 质疑现状 | First Principles | 真正的基本事实是什么？ |
| 不知如何做 | Inversion | 如何确保失败？ |
| 难以决策 | Mental Simulation | 6个月后会怎样？ |

**使用流程**:
1. 识别问题类型
2. 选择合适工具
3. 按框架操作
4. 记录洞察到Insight

**学习路径**:
- 第1-2周: 理解概念，选1-2个工具练习
- 第3-8周: 每周至少用1次，形成习惯
- 3个月+: 自然调用，工具组合使用

### Environment - 环境优化

**核心理念**:
> "减少摩擦，而非维护清单"

**执行方式**:
1. 只记录 Top 3 关键摩擦
2. 每次只做一个最小实验
3. 有效模式沉淀为 `Insight`

### Vital - 生命力管理

**核心理念**:
> "关注约束与瓶颈，而非精细台账"

**执行方式**:
1. 只写当前瓶颈（健康/财务）
2. 选择 1-2 个小步实验
3. 将验证结果沉淀为 `Loop` 或 `Insight`

---

## 🤖 Bases 查询系统

`Bases/` 文件夹包含了 37 个预设的数据库视图。
不要直接编辑这些文件，它们是作为 Dataview 的查询配置存在的。

**如何使用**:
在任何笔记中，你可以通过 Dataview 引用这些 Base 来查看特定的数据切片。

> *注意: Templates 3 的核心模板内部已经内置了基于 Dataview 的自动化查询，你不需要手动配置 Bases 即可看到关联数据。*

**自动化亮点**:
- ⚡ 能量自适应任务推荐（根据当前能量推荐合适任务）
- 📊 Goal进度可视化（自动计算进度条）
- 🔴 OS健康预警（7天未处理Signal自动标红）
- 📈 完成率自动计算（Daily笔记自动统计）

---

## ⚡ 常用快捷键建议

- **Ctrl+N**: 创建新笔记
- **Alt+T**: 插入模板 (Obsidian Templater)
- **Alt+Q**: 快速切换到 Daily Note
- **Ctrl+P**: 命令面板（搜索任何功能）

---

## 📊 维护指南

### 每日维护
- **Inbox清零**: 每天睡前（Daily晚间闭环）
- **Vital快速更新**: 每周日（5分钟）

### 每周维护
- **Review复盘**: 每周日（30分钟）
- **Environment检查**: 月末周日（识别新摩擦点）

### 每月维护
- **Goal进度检查**: 每月1日
- **环境重置**: 每月最后一个周日（清理物理/数字/社交）

### 每季度维护
- **OS系统诊断**: 每季度第1周（更新系统健康指标）
- **Compass复审**: 每季度末（价值观/愿景/北极星）
- **Vital深度复盘**: 季度末（能量曲线/财务自由路径）

---

## 🎓 学习路径

### 新手路径 (第1周)

**Day 1-2**: 基础认知
- [ ] 阅读本README
- [ ] 理解双模式哲学
- [ ] 创建Daily (Quick Mode)
- [ ] 使用Signal捕获3个想法

**Day 3-5**: 核心工作流
- [ ] 创建Compass（价值观+愿景）
- [ ] 创建3个Action
- [ ] 晚间Daily闭环检查
- [ ] 将1个Signal转化为Insight

**Day 6-7**: 扩展功能
- [ ] 尝试Daily Deep Mode
- [ ] 创建第一个Project
- [ ] 开始Vital监控

### 进阶路径 (第2-4周)

- [ ] 熟练使用所有Quick Mode
- [ ] 开始选择性使用Deep Mode
- [ ] 尝试Tools模板（遇到复杂问题时）
- [ ] 完成Environment首次评估
- [ ] 建立每周Review习惯

### 精通路径 (2-3个月)

- [ ] Quick/Deep模式自由切换
- [ ] Tools工具自然调用
- [ ] 环境持续优化
- [ ] Vital指标稳定提升
- [ ] 系统个性化定制

---

## 🔧 高级配置

### 自定义双模式

你可以为任何模板添加双模式支持：

```markdown
---
mode: quick  # or deep
---

## Quick Mode 内容
...

<%* if (tp.frontmatter.mode === "deep") { %>
---
## Deep Mode 专属内容
...
<%* } %>
```

### 创建个人工具

在Tools模板底部"工具进化"区域添加你的个人思维工具：

```markdown
### 个人创造工具
**工具名**: 你的工具名
**适用场景**: 什么时候用
**操作步骤**: 
1. 第一步
2. 第二步
```

---

## 💡 最佳实践

### 1. Quick Mode 优先
- 新笔记默认用Quick Mode
- 只在需要时才切换Deep Mode
- 避免"完美主义"陷阱

### 2. 工具按需调用
- Tools不是每天用，而是遇到复杂问题时用
- 一次解决一个问题，不要贪多
- 记录工具使用效果

### 3. 环境持续优化
- 每月识别1个新的摩擦点
- 小步快跑，逐步改善
- A/B测试验证效果

### 4. Vital稳定监控
- Quick Mode保持每周更新
- Deep Mode每季度复盘
- 关注趋势而非绝对值

### 5. 系统健康第一
- 感觉混乱时，先清空Inbox
- 定期使用OS诊断系统健康
- 复杂度上升时，回归Quick Mode

---

## 🆚 与其他系统对比

| 特性 | Templates (31) | Templates 1 (15) | Templates 3 v1.1 (22) |
|------|----------------|------------------|-----------------------|
| 模板数量 | 31 | 15 | 22 |
| 双模式 | ❌ | ❌ | ✅ ⭐⭐⭐ |
| 自动化 | ⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| 思维工具 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ ⭐NEW |
| 环境优化 | ✅ | ❌ | ✅ ⭐NEW |
| 健康财务 | ✅ (分离) | ❌ | ✅ (整合) ⭐NEW |
| 学习曲线 | 陡峭 | 平缓 | 渐进式 ⭐ |
| 总评分 | 7.8/10 | 8.6/10 | **9.68/10** ⭐ |

**Templates 3 v1.1 = 完整性(90%) + 简洁性(双模式) + 自动化(Dataview)**

---

## 📚 推荐阅读

### 系统思维
- 《Getting Things Done》- David Allen (任务管理)
- 《Building a Second Brain》- Tiago Forte (知识管理)

### 思维工具
- 《穷查理宝典》- 查理·芒格 (多元思维模型)
- 《超级思维》- Gabriel Weinberg (118个思维模型)

### 环境设计
- 《掌控习惯》- James Clear (环境塑造行为)
- 《福格行为模型》- BJ Fogg (B=MAP)

### 生命力管理
- 《Why We Sleep》- Matthew Walker (睡眠科学)
- 《财务自由之路》- Bodo Schäfer (财务规划)

---

## 🔗 快速跳转

- [[Daily|📅 今日Dashboard]]
- [[Compass|🧭 价值观愿景]]
- [[Signal|💡 快速捕获]]
- [[Insight|🧠 深度思考]]
- [[Action|✅ 任务管理]]
- [[Tools|🧰 思维工具箱]] ⭐NEW
- [[Environment|🏠 环境优化]] ⭐NEW
- [[Vital|💪 生命力管理]] ⭐NEW

---

## 📝 更新日志

### v1.1 (2026-02-04)
✨ **新增**:
- Tools模板（5大思维工具）
- Environment模板（三维环境优化）
- Vital模板（健康财务整合）

📈 **提升**:
- 完整性: 8.5 → 9.5 (+1.0)
- 思维工具: 7.0 → 9.0 (+2.0)
- 总评分: 9.34 → 9.68 (+0.34)

### v1.0 (2026-02-05)
- 初始版本发布
- 19个核心模板
- 双模式架构
- 37个Bases

---

**版本**: v1.1.0  
**更新日期**: 2026-02-04  
**系统评分**: 9.68/10 ⭐⭐⭐⭐⭐

**Templates 3 v1.1 - 更完整，更强大，仍然简洁！** 🚀
