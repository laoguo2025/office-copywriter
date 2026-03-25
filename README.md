# office-copywriter

Internal operations writing skill for enterprise administrative, HR, logistics, and general management documents.

It is designed for **internal office writing**, not external business or marketing copy.

## What it does

This skill helps generate and refine common internal enterprise documents such as:

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

It focuses on:

- choosing the right document type first
- producing a usable draft quickly
- keeping the default path short
- loading output mode / department tone only when they materially help

## Current design

The skill is organized into three layers:

### 1. Default drafting backbone
Used for most requests:

1. `references/minimal-invocation.md`
2. `references/pragmatic-scope.md`
3. `references/doc-type-routing.md`
4. matching templates and drafting prompts

### 2. On-demand enhancement layer
Only used when needed:

- output modes
- department tone refinement
- review / compliance checks
- rewrite / formalization paths

### 3. Validation layer
Used for regression and acceptance, not normal drafting:

- `validation/*`

## Key principles

- document type before polish
- usable draft before completeness
- shortest useful path first
- non-default assets should not dominate the default workflow

## Directory overview

```text
office-copywriter/
├── SKILL.md
├── README.md
├── ACCEPTANCE.md
├── CHANGELOG.md
├── prompts/
├── references/
│   └── templates/
└── validation/
```

## Suggested use cases

Use this skill when the user needs internal operations writing for:

- 行政
- 人事
- 后勤
- 综合运营

Do **not** use it for:

- marketing copy
- external sales/business copy
- public-facing brand content
- social media growth content

## Status

This skill has already been slimmed down from a heavier reference-first structure into a more practical shape:

- **default light backbone**
- **on-demand enhancements**
- **separated validation layer**

## Notes for GitHub

If publishing this folder as a repository, recommended additions are:

- a license file
- repository topics such as `openclaw`, `skill`, `writing`, `office`, `internal-documents`
- a short repo description matching the first paragraph of this README
