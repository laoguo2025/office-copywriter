# CHANGELOG

## 2026-03-25

### Added
- 补齐批复能力链：模板、prompt、示例、路由接入。
- 新增 4 个输出模式 prompt：
  - 正式发文版
  - 领导汇报版
  - 制度条款版
  - 会议落地版
- 新增文种与输出模式桥接规则：`references/document-type-output-bridge.md`
- 新增输出模式实稿验收资产：
  - `validation/notice-quick-vs-formal.md`
  - `validation/request-normal-vs-brief.md`
  - `validation/minutes-plain-vs-execution.md`
  - `validation/circular-plain-vs-formal.md`
  - `validation/regulation-plain-vs-clauses.md`
  - `validation/decision-plain-vs-formal.md`
  - `validation/plan-plain-vs-formal.md`
  - `validation/report-plain-vs-brief.md`
  - `validation/README.md`

### Changed
- 重写并清理 `SKILL.md`，修复输出模式入口不完整和脏尾部内容问题。
- 更新 `references/quickstart-commands.md`，加入输出模式快速判断。
- 更新 `references/template-example-map.md`，加入 validation 对打样例入口。
- 更新 `references/templates/examples/INDEX.md`，加入 validation 对打样例入口。

### Fixed
- 修复输出模式“有 prompt 但无组合规则”的半成品状态。
- 将输出模式桥接回归结果从 2/5 提升到 5/5。
- 修复部分索引/主说明文件的历史污染与结构不一致问题。

### Added（验收深化）
- 新增真实回归测试矩阵：`validation/routing-regression-cases.md`
- 新增真实回归结果页：`validation/routing-regression-results.md`

### Changed（导航升级）
- 将 `validation/README.md` 从“输出模式验收说明”升级为“验收资产总导航”
- 更新 `references/templates/examples/INDEX.md`，加入真实回归测试入口
- 更新 `references/template-example-map.md`，加入真实回归测试入口
- 更新 `ACCEPTANCE.md`，纳入真实回归测试阶段判断与下一步建议
- 更新 `prompts/rewrite-rough-notes.md`，加入主责部门判断与部门口径收束
- 更新 `prompts/upgrade-to-formal-version.md`，加入主责部门判断与部门味道自检
- 更新 `prompts/review-doc.md`，将部门口径判断纳入审稿维度与输出合同
- 新增 4 组边界型回归文件：请示 vs 报告、决定 vs 通知、制度 / 管理办法 vs 方案、通知 vs 通报
- 更新 `validation/README.md`、`references/templates/examples/INDEX.md`、`references/template-example-map.md`，加入边界型回归入口
- 更新 `ACCEPTANCE.md`，纳入边界型回归阶段成果与下一步建议
- 新增 `references/pragmatic-scope.md`，明确 skill 进入“够用优先、控制复杂度”的收敛阶段
- 更新 `SKILL.md`，将 pragmatic usefulness 作为默认工作原则，并把 `pragmatic-scope.md` 接入主读取路径
- 新增 `references/minimal-invocation.md`，把 skill 收敛为更短的默认使用路径
- 调整 `SKILL.md` 的读取顺序与路由规则：默认少读样例、少走长链，先给可用稿再精修
- 进一步重写 `SKILL.md` 主干：引入 `minimal-invocation.md` 作为最小默认入口，明确 secondary materials 不属于默认加载链，并清理尾部历史重复残片
- 新增 `references/one-page-navigation.md`，把主干入口、加读条件、非默认入口集中到一页
- 新增 `references/hard-slimming-candidates.md`，将现有 references / validation 分为“保留主用 / 保留但降级 / 可删除候选”三层
- 新增 `references/non-default-assets.md`，明确哪些辅助 / 精修 / 验收资产不应进入普通起草默认路径
- 继续压缩 `SKILL.md` 的 secondary materials，去掉低价值辅助文件名直列，只保留非默认原则与收敛入口
- 更新 `references/one-page-navigation.md`，进一步强化“不要默认加载次级资产”的约束
- 将 `quickstart-commands.md`、`quick-brief-schema.md` 先降级、后完成物理删除，避免历史辅助入口继续占据主骨架周边位置
- 将 `high-frequency-examples.md`、`template-example-map.md` 先降级、后完成物理删除，避免历史辅助层继续占据默认资产位置
- 将 `department-routing-rules.md`、`department-tone-baselines.md`、`department-vocabulary.md` 改写为“已收缩”的按需微调层文件，避免部门精修继续主导默认起草路径
- 清理 `ACCEPTANCE.md` 的历史脏尾巴与重复段落，收口当前阶段判断
