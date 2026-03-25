# office-copywriter｜Acceptance Summary

## 本轮目标
把 `office-copywriter` 从“有模板、有路由”推进到“输出模式可控、可验收、可维护”的可实战状态。

## 本轮完成项

### 1. 批复能力链补齐
已补齐：
- `references/templates/reply-approval.md`
- `prompts/draft-reply-approval.md`
- `references/templates/examples/reply-approval-procurement-example.md`

并已接入：
- `references/doc-type-routing.md`
- `references/usage-scenario-map.md`
- `references/templates/examples/INDEX.md`
- `SKILL.md`

### 2. 输出模式层补齐
已新增 4 个独立 output-mode prompt：
- `prompts/output-formal-issuance.md`
- `prompts/output-leadership-brief.md`
- `prompts/output-regulation-clauses.md`
- `prompts/output-meeting-execution.md`

### 3. 文种 × 输出模式桥接层补齐
已新增：
- `references/document-type-output-bridge.md`

用于明确：
- 通知默认快速稿，正式下发时切正式发文版；
- 请示默认快速稿，面向领导审批时切领导汇报版；
- 批复默认正式发文版；
- 制度默认制度条款版；
- 会议纪要默认会议落地版。

### 4. 实稿验收资产补齐
已新增：
- `validation/notice-quick-vs-formal.md`
- `validation/request-normal-vs-brief.md`
- `validation/minutes-plain-vs-execution.md`
- `validation/README.md`

并已回挂到：
- `references/templates/examples/INDEX.md`
- `SKILL.md`

## 验收结果

### 一、文种/路由回归
此前已完成：12/12 通过。
覆盖场景包括：
- 放假安排
- 采购申请
- 审批回复
- 阶段汇报
- 会议纪要
- 通报
- 决定
- 制度
- 方案
- 工作计划
- 总结
- 情况说明

### 二、输出模式桥接回归
本轮从 2/5 修复到 5/5 通过。
最终通过项：
- 通知 + 快速可用稿
- 通知 + 正式发文版
- 请示 + 领导汇报版
- 制度 + 制度条款版
- 会议纪要 + 会议落地版

### 三、实稿差异验收
已完成 8 组实稿对打：
- 通知：快速稿 vs 正式发文版
- 请示：普通稿 vs 领导汇报版
- 会议纪要：普通整理 vs 会议落地版
- 通报：普通说明稿 vs 正式发文版
- 制度：普通说明稿 vs 制度条款版
- 决定：普通稿 vs 正式发文版
- 方案：普通稿 vs 正式发文版
- 报告：普通稿 vs 领导汇报版

结论：
- 快速稿与正式发文版差异明确；
- 普通请示与领导汇报版差异明确；
- 普通纪要与会议落地版差异明确；
- 普通通报与正式发文版差异明确；
- 普通制度说明与制度条款版差异明确；
- 普通决定与正式发文版差异明确；
- 普通方案与正式发文版差异明确；
- 普通报告与领导汇报版差异明确。

### 5. 部门口径精修基线补齐
已新增：
- `references/department-tone-baselines.md`

作用：
- 将“行政 / 人事 / 后勤 / 综合运营”四类部门口径，从原先的词汇偏好，推进到“关注点 + 语言气质 + 动作词 + 常见句型 + 不同输出模式下的微调建议”的统一基线；
- 为下一阶段的“同题不同部门”实稿对打提供共同参考底稿；
- 避免部门真实感继续停留在零散用词层面。

并已接入：
- `SKILL.md`
- `ACCEPTANCE.md`

### 6. 同题不同部门实稿对打首组落地
已新增：
- `validation/notice-same-topic-by-department.md`

内容：
- 以“清明节前后工作安排通知”为同一题目；
- 分别产出行政 / 人事 / 后勤 / 综合运营 4 个版本；
- 用同题对打方式验证部门口径差异不再只停留在词汇层，而是能体现到关注点、要求表达和成稿气质。

并已回挂到：
- `validation/README.md`
- `references/templates/examples/INDEX.md`

### 7. 同题不同部门第二组落地（情况说明）
已新增：
- `validation/explanation-same-topic-by-department.md`

内容：
- 以“员工安全培训签到数据不一致情况说明”为同一题目；
- 分别产出行政 / 人事 / 后勤 / 综合运营 4 个版本；
- 重点验证“情况说明”这类更容易写成统一模板口径的文种，是否能在解释重点、责任边界、整改表达上形成部门差异。

并已回挂到：
- `validation/README.md`
- `references/templates/examples/INDEX.md`

### 8. 同题不同部门第三组落地（工作计划）
已新增：
- `validation/work-plan-same-topic-by-department.md`

内容：
- 以“4月月度重点工作计划”为同一题目；
- 分别产出行政 / 人事 / 后勤 / 综合运营 4 个版本；
- 重点验证“工作计划”这类容易写成空泛套话的文种，是否能在工作重心、推进方式、保障表达上形成部门差异。

并已回挂到：
- `validation/README.md`
- `references/templates/examples/INDEX.md`

### 9. 部门口径调用规则固化
已新增：
- `references/department-routing-rules.md`

作用：
- 将“部门口径精修”从样例层推进到调用层；
- 明确在真实 drafting / rewrite 时，什么时候优先按行政、人事、后勤、综合运营口径起稿；
- 补齐易混淆边界（如行政 vs 综合运营、人事 vs 行政、后勤 vs 行政等）的判断规则；
- 形成“场景识别 → 主责部门判断 → 部门口径路由 → 语言微调 → 实稿校验”的默认路径。

并已接入：
- `SKILL.md`
- `ACCEPTANCE.md`

### 10. 部门口径规则下沉到高频 drafting prompt
已更新：
- `prompts/draft-notice.md`
- `prompts/draft-summary.md`
- `prompts/draft-work-plan.md`

作用：
- 不再只在参考层说明部门差异，而是把部门口径判断直接写入高频起草 prompt；
- 让“通知 / 情况说明 / 工作计划”三类高频文种在真实执行时，优先按主责部门口径收束，而不是事后靠人工补救；
- 把 `department-routing-rules.md`、`department-tone-baselines.md`、`department-vocabulary.md` 变成 prompt 执行时的直接参考依赖。

### 11. 部门口径规则继续下沉到第二批高频 prompt
已更新：
- `prompts/draft-report.md`
- `prompts/draft-request.md`
- `prompts/draft-circular.md`

作用：
- 将部门口径判断从第一批高频文种继续扩展到报告、请示、通报；
- 让“报告 / 请示 / 通报”在真实起草时，也会先按主责部门识别汇报重点、请批理由、警示导向；
- 进一步减少“参考层很强、但执行层还是统一模板口气”的风险。

### 12. 第三批高频 drafting prompt 补齐并下沉部门口径
已新增/更新：
- `prompts/draft-minutes.md`（新增）
- `prompts/draft-regulation.md`（新增）
- `prompts/draft-decision.md`（补充部门口径下沉）

作用：
- 补齐此前缺失的会议纪要与制度类 drafting prompt；
- 让“会议纪要 / 制度 / 决定”也进入按主责部门自动收束的执行路径；
- 使部门口径下沉从前两批高频文种进一步扩展到第三批核心内部文种。

### 13. 文种 × 输出模式 × 部门口径总导航补齐
已新增：
- `references/department-routing-quickstart.md`

作用：
- 把文种选择、输出模式选择、部门口径判断整合成一个快速导航入口；
- 提供最常用组合与推荐读取顺序，减少在多份参考文件之间跳转；
- 将 `office-copywriter` 的调用方式从“知道很多资产”推进到“有统一入口可以直接用”。

并已接入：
- `SKILL.md`
- `ACCEPTANCE.md`

### 14. 真实回归测试矩阵补齐
已新增：
- `validation/routing-regression-cases.md`
- `validation/routing-regression-results.md`

作用：
- 用 12 个高混淆真实题目，系统验证 skill 是否能够默认选对文种、输出模式和主责部门口径；
- 把当前阶段判断从“资料补齐”推进到“规则级回归已建立”；
- 明确下一阶段的缺口不再是主干建设，而是边界型回归和 rewrite/review 链下沉部门口径。

并已回挂到：
- `validation/README.md`
- `references/templates/examples/INDEX.md`

### 15. rewrite / formalize / review 三条链补齐部门口径下沉
已更新：
- `prompts/rewrite-rough-notes.md`
- `prompts/upgrade-to-formal-version.md`
- `prompts/review-doc.md`

作用：
- 让“草稿改正式、口语转成稿、审稿纠偏”三条实战链，不再只判断文种，还会显式判断主责部门；
- 将行政 / 人事 / 后勤 / 综合运营的口径差异，从 drafting 层进一步扩展到 rewrite / review 层；
- 降低真实使用中“文种对了，但部门味道还是中性模板稿”的风险。

## 当前成熟度判断
`office-copywriter` 当前已达到：

**可实战交付**

具体表现为：
- 能稳定判断文种；
- 能按输出目标切换成稿形态；
- 有桥接规则，不再依赖隐含经验；
- 有实稿验收样例可回看；
- 有索引入口，后续维护成本更低；
- 已建立真实回归测试矩阵，开始具备“默认路径是否真可用”的验收能力。

同时，本轮也明确了一个收敛判断：
- 这份 skill 的后续目标应是**更好用**，不是**更复杂**；
- 企业个性化文风不应继续大量预埋进 skill；
- skill 更适合保留“共性骨架”，把企业差异留到运行时约束。

并已进一步补上三类收敛资产：
- `references/minimal-invocation.md`
- `references/one-page-navigation.md`
- `references/hard-slimming-candidates.md`

作用：
- 让使用者优先按“先文种、再可用稿、缺什么补什么”的最短路径使用；
- 明确哪些企业差异应在调用时补一句，而不是继续预埋到 skill 里；
- 把复杂能力收敛为更容易落地的默认使用方式；
- 为下一步硬瘦身提供“保留主用 / 保留但降级 / 可删除候选”的明确分级。

## 后续建议（非本轮阻塞项）
1. 进入收敛阶段，优先维护主骨架清晰度，不再默认扩展细颗粒企业文风规则；
2. 如果后续继续补验收，应优先验证“现有骨架是否更好用”，而不是继续增加覆盖面；
3. 下一步硬瘦身应优先处理重复导航与低价值辅助层，再视引用情况决定是否真正删除文件。

## 本轮可复用经验
- 对高频 skill，单补 prompt 不够，必须同步补：
  1. 路由层
  2. 桥接层
  3. 实稿验收层
  4. 索引回挂层
- 当 skill 开始接近“越做越复杂”的临界点时，应主动做一次收敛判断：保留高价值共性，停止低收益细化。
- 如果索引类 Markdown 出现脏编码或历史污染，优先整文件重写，不要继续做局部 patch。
