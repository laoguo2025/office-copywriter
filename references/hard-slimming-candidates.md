# hard-slimming-candidates（当前态）

## 目的
这份文件不再记录已经完成的删除历史，而是只保留 **当前还值得继续观察的硬瘦身对象**。

原则：
- 不为了“看起来完整”保留默认不该读的材料；
- 不动主骨架；
- 优先处理会继续增加默认理解成本、但又不直接提升默认成功率的文件；
- 已经完成删除的文件不再留在候选区反复出现。

---

## A. 主骨架（不动）
这些文件现在直接承担默认可用性，不进入候选。

### 默认入口 / 主判断
- `references/minimal-invocation.md`
- `references/one-page-navigation.md`
- `references/pragmatic-scope.md`
- `references/doc-type-routing.md`
- `references/usage-scenario-map.md`
- `references/doc-boundary-rules.md`
- `references/direction-rules.md`

### 质量与合规底线
- `references/review-checklist.md`
- `references/format-rules.md`
- `references/tone-rules.md`
- `references/internal-vs-external.md`
- `references/common-mistakes.md`

### 输出模式主骨架
- `references/output-modes.md`
- `references/document-type-output-bridge.md`

### 模板层
- `references/templates/*`

### 执行 prompt 层
- `prompts/draft-*.md`
- `prompts/rewrite-rough-notes.md`
- `prompts/upgrade-to-formal-version.md`
- `prompts/review-doc.md`
- `prompts/output-*.md`

---

## B. 保留但继续后置
这些文件仍有价值，但默认不该读。

### 部门微调层
- `references/department-routing-quickstart.md`
- `references/department-routing-rules.md`
- `references/department-tone-baselines.md`
- `references/department-vocabulary.md`

当前判断：
- 保留；
- 只在部门口径确实影响成稿时进入；
- 不再视为主骨架的一部分。

### 验收 / 回归层
- `validation/README.md`
- `validation/routing-regression-cases.md`
- `validation/routing-regression-results.md`
- 其余 `validation/*.md`

当前判断：
- 对验收有价值；
- 对普通起草不是默认必要；
- 应继续与调用层分离。

---

## C. 当前仍值得观察的候选
这部分才是下一轮真正可能继续收的对象。

### 第一优先级候选
- `references/rewrite-modes.md`

原因：
- 仍偏“辅助说明页”，不是直接执行主骨架；
- 与 `prompts/rewrite-rough-notes.md` / `prompts/upgrade-to-formal-version.md` / `prompts/review-doc.md` 存在职责重叠；
- 如果继续保留，应明确为二级索引，而不是默认路径旁的解释层。

建议：
- 先收缩，不急着删；
- 若后续发现几乎不再提供独立价值，可再考虑归档或删除。

### 第二优先级候选
- `validation/README.md`

原因：
- 如果后续验收入口已经能由更短的导航承担，这份 README 可能变成重复导航层；
- 但现阶段仍有组织作用，不建议现在就删。

---

## D. 已完成项（不再反复挂候选）
以下文件已完成物理删除，不再保留在候选区：
- `references/high-frequency-examples.md`
- `references/template-example-map.md`
- `references/quickstart-commands.md`
- `references/quick-brief-schema.md`

---

## 当前结论
`office-copywriter` 下一轮若继续硬收，重点不再是“大面积删文件”，而是：
1. 继续压低二级说明层的存在感；
2. 保持默认主骨架短而稳；
3. 让验收层继续远离默认调用；
4. 只处理仍然会制造默认复杂感、但贡献有限的剩余对象。
