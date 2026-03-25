# office-copywriter

面向企业内部使用的办公写作 Skill，主要服务于**行政、人事、后勤、综合运营**等场景下的常见文书起草、改写与规范化输出。

> A practical OpenClaw skill for internal office writing in Chinese enterprise contexts, focused on administrative, HR, logistics, and general operations documents.

## 中文说明

### 这个 Skill 是干什么的

`office-copywriter` 用来处理企业内部常见办公文书，重点不是“堆模板”，而是：

- 先判断**文种**是否正确
- 先给出**能直接用的初稿**
- 默认路径尽量短，避免一上来读太多资料
- 只有在确实需要时，才追加**输出模式**和**部门口径**修正

它适合处理的典型内容包括：

- 通知
- 请示
- 批复
- 报告
- 会议纪要
- 通报
- 决定
- 制度 / 管理办法
- 方案 / 实施方案
- 工作计划
- 总结 / 情况说明
- 常见内部表单 / 单据类文书

---

### 适用范围

适用于企业内部办公写作，尤其是这些方向：

- 行政
- 人事
- 后勤
- 综合运营

不适用于：

- 市场营销文案
- 对外销售/商务文案
- 品牌宣传内容
- 社交媒体增长内容

一句话说，就是：

> **它是内部运营管理写作 Skill，不是外部商业文案 Skill。**

---

### 当前设计思路

这个 Skill 现在已经从“资料很多、路径偏重”的状态，收敛成了一个更适合实战的三层结构：

#### 1）默认主骨架层
日常起草优先走这条最短路径：

1. `references/minimal-invocation.md`
2. `references/pragmatic-scope.md`
3. `references/doc-type-routing.md`
4. 对应模板与 drafting prompts

这一层的目标很明确：

- 先把文种选对
- 先把草稿写出来
- 先交付最简单可用版本

#### 2）按需增强层
只有在场景确实需要时才进入：

- 输出模式调整
- 部门口径微调
- 审核 / 合规检查
- 改写 / 转正式 / 审稿链路

这一层不是默认入口，而是增强层。

#### 3）验收 / 回归层
用于验证 skill 是否还能稳定判断和输出，不是默认起草路径：

- `validation/*`

---

### 这个 Skill 的核心原则

- **文种优先于润色**
- **可用初稿优先于表面完整**
- **最短可用路径优先**
- **非默认资产不应主导默认工作流**

也就是说，它不是一个“每次都先读一堆规则”的 Skill，
而是一个**先出结果，再按需增强**的 Skill。

---

### 目录结构

```text
office-copywriter/
├── SKILL.md
├── README.md
├── LICENSE
├── ACCEPTANCE.md
├── CHANGELOG.md
├── prompts/
├── references/
│   └── templates/
└── validation/
```

---

### 当前状态

目前这个 Skill 的状态可以概括为：

- **默认轻骨架**
- **增强层按需调用**
- **验收层独立存在**

也就是说，它已经不再是“继续堆文件”的阶段，
而是进入了**可直接实战交付**的状态。

---

### GitHub 展示说明

因为这个仓库主要面向中文办公场景，所以 README 采用：

- **中文优先**
- **英文摘要补充**
- 不做整篇逐段镜像翻译

这样更符合实际使用人群，也更适合 GitHub 展示。

---

## English Overview

`office-copywriter` is an OpenClaw skill for **internal enterprise office writing**, especially in Chinese business environments.

It is designed to help with documents such as notices, requests, reports, minutes, decisions, regulations, plans, summaries, explanations, and common internal forms.

### What makes it practical

Instead of loading too many references by default, the skill now follows a lighter workflow:

1. identify the correct **document type** first
2. generate a **usable draft** quickly
3. apply **output mode** or **department tone** only when needed

### Current structure

- **Default drafting backbone** for the shortest useful path
- **On-demand enhancement layer** for refinement and review
- **Validation layer** for regression and acceptance checks

### Best fit

Best used for internal writing in:

- administration
- HR
- logistics
- general operations

Not intended for:

- marketing copy
- external business copy
- brand-facing content
- social media growth content
