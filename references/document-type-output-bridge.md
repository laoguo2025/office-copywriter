# document-type-output-bridge（文种与输出模式桥接）

## 目的
把“文种 prompt”与“输出模式 prompt”连接起来，避免只知道文种或只知道模式，却不知道两者如何组合。

## 总原则
1. 先确定文种。
2. 再确定输出模式。
3. 默认先用对应文种 prompt 打底，再按需要叠加 output-mode prompt 调整成稿形态。
4. 若用户未明确提出输出模式，则按该文种的默认输出模式处理。

---

## 1. 通知
- 文种 prompt：`prompts/draft-notice.md`
- 默认输出模式：快速可用稿
- 若用户说“正式一点 / 内部下发 / 发文 / 留档” → 叠加：`prompts/output-formal-issuance.md`
- 若用户没说模式、但明显要直接发出 → 优先按正式发文版处理

## 2. 请示
- 文种 prompt：`prompts/draft-request.md`
- 默认输出模式：快速可用稿
- 若用户说“给领导看 / 汇报版 / 压缩重点 / 领导审阅” → 叠加：`prompts/output-leadership-brief.md`
- 若用户没说模式，但明显面向领导审批 → 优先按领导汇报版处理

## 3. 批复
- 文种 prompt：`prompts/draft-reply-approval.md`
- 默认输出模式：正式发文版
- 默认叠加：`prompts/output-formal-issuance.md`

## 4. 报告 / 情况说明 / 总结
- 文种 prompt：`prompts/draft-report.md` 或对应总结/说明路径
- 默认输出模式：快速可用稿
- 若用户说“给领导看 / 汇报重点 / 要结论版” → 叠加：`prompts/output-leadership-brief.md`
- 若用户没说模式，但受众明显是领导 → 优先按领导汇报版处理

## 5. 会议纪要
- 文种 prompt：会议纪要对应路径
- 默认输出模式：会议落地版
- 默认叠加：`prompts/output-meeting-execution.md`

## 6. 制度 / 管理办法
- 文种 prompt：制度 / 办法对应路径
- 默认输出模式：制度条款版
- 默认叠加：`prompts/output-regulation-clauses.md`

## 7. 通报 / 决定 / 方案 / 工作计划
- 先按文种模板起稿
- 默认输出模式：快速可用稿
- 若用户强调“正式下发 / 统一口径 / 留档执行” → 叠加：`prompts/output-formal-issuance.md`

---

## 快速判断句
- 通知：先写通知，再决定是“快速稿”还是“正式发文版”
- 请示/报告：先写请示/报告，再决定是否压成“领导汇报版”
- 制度：默认直接走“制度条款版”
- 纪要：默认直接走“会议落地版”

## 使用提醒
- output-mode prompt 不是替代文种 prompt，而是对成稿形态做二次收束。
- 除制度条款版、会议落地版、批复正式发文版这类强默认组合外，其余优先采用“文种 prompt 打底 + 模式 prompt 调整”的方式。
