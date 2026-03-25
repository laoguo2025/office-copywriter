# examples/INDEX（完整示例索引）

## 按部门查看

### 行政
- `admin-notice-example.md` — 春节放假安排通知（通知 / 正式发文版）
- `procurement-request-example.md` — 办公设备采购请示（请示 / 领导汇报版）
- `reply-approval-procurement-example.md` — 采购申请批复（批复 / 正式发文版）
- `office-supplies-policy-example.md` — 办公用品管理办法（制度 / 制度条款版）

### 人事
- `hr-notice-example.md` — 员工调岗通知（通知 / 正式发文版）
- `request-staffing-example.md` — 招聘编制申请请示（请示 / 领导汇报版）
- `decision-appointment-example.md` — 任命决定（决定 / 正式发文版）
- `training-plan-example.md` — 年度培训实施方案（方案 / 正式发文版）
- `attendance-circular-example.md` — 考勤异常情况通报（通报 / 正式发文版）

### 后勤
- `logistics-report-example.md` — 食堂整改情况报告（报告 / 领导汇报版）
- `safety-circular-example.md` — 安全检查情况通报（通报 / 正式发文版）
- `dormitory-policy-example.md` — 员工宿舍管理办法（制度 / 制度条款版）

### 综合运营
- `ops-minutes-example.md` — 跨部门流程优化协调会会议纪要（会议纪要 / 会议落地版）
- `monthly-work-plan-example.md` — 综合运营部月度重点工作计划（工作计划 / 正式发文版）

## 按文种查看
- 通知：`admin-notice-example.md`、`hr-notice-example.md`
- 请示：`request-staffing-example.md`、`procurement-request-example.md`
- 批复：`reply-approval-procurement-example.md`
- 报告：`logistics-report-example.md`
- 会议纪要：`ops-minutes-example.md`
- 通报：`safety-circular-example.md`、`attendance-circular-example.md`
- 决定：`decision-appointment-example.md`
- 制度 / 办法：`dormitory-policy-example.md`、`office-supplies-policy-example.md`
- 方案：`training-plan-example.md`
- 工作计划：`monthly-work-plan-example.md`
- 总结：`work-summary-example.md`
- 情况说明：`incident-explanation-example.md`
- 内部协同函式沟通：`internal-coordination-letter-example.md`

## 输出模式验收样例（validation）
- `../../validation/notice-quick-vs-formal.md` — 同一通知题目下，快速可用稿 vs 正式发文版
- `../../validation/request-normal-vs-brief.md` — 同一请示题目下，普通稿 vs 领导汇报版
- `../../validation/minutes-plain-vs-execution.md` — 同一纪要题目下，普通整理 vs 会议落地版
- `../../validation/circular-plain-vs-formal.md` — 同一通报题目下，普通说明稿 vs 正式发文版
- `../../validation/regulation-plain-vs-clauses.md` — 同一制度题目下，普通说明稿 vs 制度条款版
- `../../validation/decision-plain-vs-formal.md` — 同一决定题目下，普通稿 vs 正式发文版
- `../../validation/plan-plain-vs-formal.md` — 同一方案题目下，普通稿 vs 正式发文版
- `../../validation/report-plain-vs-brief.md` — 同一报告题目下，普通稿 vs 领导汇报版
- `../../validation/notice-same-topic-by-department.md` — 同一通知题目下，行政 / 人事 / 后勤 / 综合运营口径对打
- `../../validation/explanation-same-topic-by-department.md` — 同一情况说明题目下，行政 / 人事 / 后勤 / 综合运营口径对打
- `../../validation/work-plan-same-topic-by-department.md` — 同一工作计划题目下，行政 / 人事 / 后勤 / 综合运营口径对打
- `../../validation/routing-regression-cases.md` — 高混淆真实题目回归矩阵（12 个 case）
- `../../validation/routing-regression-results.md` — 当前真实回归结果与缺口判断
- `../../validation/request-vs-report-boundary.md` — 请示 vs 报告 边界回归
- `../../validation/decision-vs-notice-boundary.md` — 决定 vs 通知 边界回归
- `../../validation/regulation-vs-plan-boundary.md` — 制度 / 管理办法 vs 方案 边界回归
- `../../validation/notice-vs-circular-boundary.md` — 通知 vs 通报 边界回归

## 使用建议
- 用户要“直接发”的内部通知 / 决定 / 通报，优先参考正式发文版示例。
- 用户要“给领导看”的请示 / 报告，优先参考领导汇报版示例。
- 用户要“会议内容整理成能执行的结果”，优先参考会议落地版示例。
- 用户要制度类文本，优先参考制度条款版示例。
- 如需快速理解不同输出模式的实际差异，先看 `validation/` 下的对打样例。
- 用户要月度 / 年度安排类文本，优先参考工作计划或方案示例，先区分“周期性计划”还是“专项实施方案”。
