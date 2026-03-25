# validation（验收资产总导航）

这里存放 `office-copywriter` 的验收资产，不再只限于“输出模式对打”。
当前主要覆盖三类验证：
- **输出模式验收**：同一题目在不同输出模式下，是否真的形成不同成稿形态；
- **部门口径验收**：同一题目在行政 / 人事 / 后勤 / 综合运营口径下，是否真的形成差异；
- **真实回归测试**：面对高混淆题目时，是否能默认选对文种、模式与部门口径。

## 一、输出模式验收样例
- `notice-quick-vs-formal.md` — 通知：快速可用稿 vs 正式发文版
- `request-normal-vs-brief.md` — 请示：普通稿 vs 领导汇报版
- `minutes-plain-vs-execution.md` — 会议纪要：普通整理 vs 会议落地版
- `circular-plain-vs-formal.md` — 通报：普通说明稿 vs 正式发文版
- `regulation-plain-vs-clauses.md` — 制度：普通说明稿 vs 制度条款版
- `decision-plain-vs-formal.md` — 决定：普通稿 vs 正式发文版
- `plan-plain-vs-formal.md` — 方案：普通稿 vs 正式发文版
- `report-plain-vs-brief.md` — 报告：普通稿 vs 领导汇报版

## 二、部门口径验收样例
- `notice-same-topic-by-department.md` — 通知：同一题目下的行政 / 人事 / 后勤 / 综合运营口径对打
- `explanation-same-topic-by-department.md` — 情况说明：同一题目下的行政 / 人事 / 后勤 / 综合运营口径对打
- `work-plan-same-topic-by-department.md` — 工作计划：同一题目下的行政 / 人事 / 后勤 / 综合运营口径对打

## 三、真实回归测试
- `routing-regression-cases.md` — 高混淆真实题目回归矩阵（12 个 case）
- `routing-regression-results.md` — 当前规则级回归结果与缺口判断

## 四、边界型回归
- `request-vs-report-boundary.md` — 请示 vs 报告
- `decision-vs-notice-boundary.md` — 决定 vs 通知
- `regulation-vs-plan-boundary.md` — 制度 / 管理办法 vs 方案
- `notice-vs-circular-boundary.md` — 通知 vs 通报

## 怎么用
1. 先看 `references/doc-type-routing.md` 与 `references/doc-boundary-rules.md`，确认文种判断；
2. 再看 `references/output-modes.md` 与 `references/document-type-output-bridge.md`，确认模式选择；
3. 再看 `references/department-routing-rules.md` 与 `references/department-tone-baselines.md`，确认部门口径；
4. 最后回到这里看验收资产，确认差异是否足够明显、默认路径是否真的可用。

## 当前结论
- 输出模式桥接已补齐；
- 部门口径对打已形成三组主骨干样例；
- 真实回归测试矩阵已建立，skill 已进入“验收 + 补边界”阶段；
- 这些文件主要用于验收和回归，不替代模板本身。
