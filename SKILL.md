---
name: office-copywriter
description: Internal operations writing skill for enterprise administrative, HR, logistics, and general management documents. Use when the user needs 企业内部运营管理文案、行政、人事、后勤、综合管理中的内部通知、请示、批复、报告、纪要、通报、决定、制度、方案、总结、情况说明等。 Only for internal management operations, not external business writing.
---

# office-copywriter

## What this skill is
A focused writing skill for enterprise internal operations management documents:
- 企业内部运营管理文案
- 行政 / 人事 / 后勤 / 综合管理文书
- 内部通知、请示批复、汇报、纪要、制度、方案、总结、情况说明
- 只服务内部管理，不服务外部业务

It is for documents that need:
- 文种正确
- 结构完整
- 语气规范
- 可执行、可流转、可留档

## What this skill is NOT
Do not use this skill for external business or general marketing/content writing.
Not for:
- 客户沟通文案
- 商务合作文案
- 对外邀请函 / 催款函 / 商洽函
- 品牌宣传文案
- 小红书 / 抖音 / 公众号营销内容
- 销售页 / 增长文案
- PMM / 竞品分析
- 日记 / 学习笔记 / 随笔

## Default working style
- Follow user language automatically
- Prefer direct usable draft over abstract advice
- When the user gives too little info, prefer `可用初稿 + 缺失信息清单`
- Ask at most one key clarification when needed
- Prefer standard internal office structure over fancy expression
- Keep the wording正式、简明、可执行
- Default to internal management context unless the user explicitly says otherwise
- Prefer pragmatic usefulness over completeness
- First solve: 文种、方向、可用结构； then refine output mode / department tone only if they materially improve the draft

## Start here
### Minimal default path
Read in this order:
1. `references/minimal-invocation.md`
2. `references/pragmatic-scope.md`
3. `references/doc-type-routing.md`
4. matching template under `references/templates/`

Only load more references if the first draft is still uncertain or the user explicitly asks for a different form.

### If the user gave a scenario but not the document type
Then add:
5. `references/usage-scenario-map.md`
6. `references/direction-rules.md`

### If output mode or department tone clearly matters
Then add only what is needed:
- `references/output-modes.md`
- `references/document-type-output-bridge.md`
- `references/department-routing-quickstart.md`

### If quality / compliance needs checking
Read as needed, not all at once:
- `references/review-checklist.md`
- `references/doc-boundary-rules.md`
- `references/format-rules.md`
- `references/tone-rules.md`
- `references/internal-vs-external.md`
- `references/common-mistakes.md`

### Secondary materials (not default)
Use only when the draft still needs extra precision or when doing acceptance / comparison work:
- `references/department-routing-rules.md`
- `references/department-tone-baselines.md`
- `references/department-vocabulary.md`

Non-default auxiliary / validation assets should not be loaded in ordinary drafting unless clearly needed. See:
- `references/one-page-navigation.md`
- `references/hard-slimming-candidates.md`

## Routing rules (short form)
1. If the user explicitly says the document type, honor it first.
2. Else infer the document type from the internal operations scenario.
3. If the scenario maps cleanly to one document type, draft directly.
4. If multiple document types are plausible, use `references/doc-boundary-rules.md` first, then ask only one key question if ambiguity remains.
5. When the user gives only a rough scenario, prefer minimum viable completion: infer the likely document and produce `可用初稿 + 待补信息`.
6. If the user provides drafts, meeting notes, chat logs, or rough spoken material, choose the rewrite / review / formalize path first; do not over-route through extra references unless needed.
7. Use direction rules to correct tone and structure:
   - 上行文：请示 / 报告
   - 下行文：通知 / 决定 / 通报 / 批复
   - 内部平行协同场景：可参考函式正式沟通语气，但不把外部商务函作为主路径
8. Department tone is a secondary refinement, not the primary goal. Use it only when it materially changes the draft.
9. Output modes are optional refinements. If the user did not ask for one, default to the simplest usable form.
10. If the user asks to检查、润色、审稿、改正式, use `references/review-checklist.md` as the final gate before output.
11. When the task is close to direct drafting or rewrite work, prefer the prompt assets under `prompts/` as the immediate execution layer.
12. Output should favor executable office writing, not literary polish.

## Core document scope
High-frequency types for v1:
- 通知
- 请示
- 批复
- 报告
- 会议纪要
- 通报
- 决定
- 制度 / 管理办法
- 工作方案 / 实施方案
- 工作计划
- 工作总结 / 情况说明

Primary internal domains:
- 行政
- 人事
- 后勤
- 综合运营管理

## Commands
- `/oc quick-brief`
- `/oc type=通知`
- `/oc type=请示`
- `/oc type=批复`
- `/oc type=报告`
- `/oc type=会议纪要`
- `/oc type=通报`
- `/oc type=决定`
- `/oc type=制度`
- `/oc type=方案`
- `/oc type=工作计划`
- `/oc type=总结`

## Prompt assets
Drafting:
- `prompts/draft-notice.md`
- `prompts/draft-request.md`
- `prompts/draft-reply-approval.md`
- `prompts/draft-report.md`
- `prompts/draft-minutes.md`
- `prompts/draft-circular.md`
- `prompts/draft-decision.md`
- `prompts/draft-regulation.md`
- `prompts/draft-work-plan.md`
- `prompts/draft-summary.md`

Refine / convert:
- `prompts/rewrite-rough-notes.md`
- `prompts/upgrade-to-formal-version.md`
- `prompts/review-doc.md`

Output-mode refinements:
- `prompts/output-formal-issuance.md`
- `prompts/output-leadership-brief.md`
- `prompts/output-regulation-clauses.md`
- `prompts/output-meeting-execution.md`

## Practical note
This skill is now in convergence / maintenance mode.
Default goal: make it easier to use, not broader or heavier.
If a refinement mainly adds reading cost, branching cost, or maintenance cost but does not clearly improve default success rate, do not treat it as a priority improvement.
