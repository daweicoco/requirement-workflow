# PMCOCO 需求分析工作流技能

这是一个可独立使用的 Codex skill，用于把工作区中的原始需求材料、已有草稿、任务设计稿、调研记录等内容，收敛为可交接设计和开发的结构化输出。

## 这个 skill 做什么

这个 skill 采用一套分层收敛的需求分析与方案设计工作流：

1. 先收敛目标与范围
2. 再定义角色与流程
3. 再梳理数据源与结构化字段
4. 最后沉淀为系统链路、模块、状态、验收与开发交接说明

它被设计为独立可用版本，即使没有安装其他 PM skill 或写作 skill，也能够完整工作。

## 最适合的使用场景

这个 skill 最适合的不是从零空白写一篇文档，而是基于工作区已有材料做分层收敛。

典型场景包括：

- 项目文件夹里已经有原始需求文档、PRD 草稿、任务设计稿、调研材料、会议纪要等上下文
- 团队希望把零散材料整理成可以继续交给设计和开发的结构化方案
- 项目处于 Demo、PoC、MVP 阶段，需要优先形成最小闭环
- 需求分析必须体现角色、流程闭环、数据链路和下游协作，而不只是列功能点

## 推荐的前序输入材料

以下输入对本 skill 最有帮助：

- 原始需求文档，描述业务诉求、问题背景或项目目标
- 已有 PRD 草稿，格式可以是 markdown、docx 导出文本、rtf 导出文本
- task design / data-source design 一类文档，用于承接数据源、接入方式、实现思路等信息
- 调研记录、会议纪要、workshop 输出、分析摘要
- 表格类材料，例如数据源清单、样例记录、字段映射、筛选规则
- 任何已经体现角色设计、流程思路、模块假设的中间稿

## 推荐的上下文提供顺序

1. 主原始需求文档或项目需求说明
2. 最新版本的 PRD 或结构化草稿
3. task design 或 data-source design 文档
4. 会议纪要、调研笔记、分析材料
5. 表格、样例数据、字段定义、来源清单

如果只能给一个输入，通常最适合的是最新版本的结构化需求文档。

如果能给多个输入，通常效果最好的是这三个组合：

- 原始需求说明
- 最新结构化草稿
- 至少一份数据/任务设计文档

## 目录结构

- `SKILL.md`：主工作流说明
- `agents/openai.yaml`：技能展示元数据
- `references/workflow-method.md`：方法论正文
- `references/dependency-review.md`：独立打包原因说明
- `references/handoff-checklist.md`：交付检查清单
- `assets/output-template.md`：推荐输出模板

## 使用方式

将本目录放入本地 Codex skills 目录后，在新对话中显式调用本 skill。

示例：

`Use $pmcoco-requirement-workflow to analyze the current workspace requirement documents and produce a handoff-ready output for design and development.`

或者中文表达：

- 用 `pmcoco-requirement-workflow` 分析当前工作区需求文档，并输出可交接设计和开发的结构化方案。

## 说明

这个 skill 被设计成独立版，因此把关键的方法、模板和交付要求都直接打包进来了，而不是假设使用者已经安装了其他 PM skill 或写作 skill。
