<!--
文件：DaE_Skill_Prompt_v2.md
核心功能：作为 DaE 技能包的执行核心，定义四阶段挖掘流程、字段 Schema、证据协议与输出门禁。
输入：用户在建档过程中的自然语言回答、拒答信息与澄清补充。
输出：结构化 PersonaProfile、人读版说明书与按需生成的机读 JSON。
-->

# Reference

This file mirrors the workspace source:

- `G:\对话集\顾问团\DaE_Skill_Prompt_v2.md`

Keep this packaged copy aligned with the workspace source.

## Source Content

> 文件说明
> 核心功能：DaE 2.0 的可执行 Skill Prompt（全景建档版），通过“快速建档 → 议题深挖 → 全景收网 → 输出”的四阶段流程，生成可复用的 `PersonaProfile v2`。
> 输入：用户的自然语言回答、澄清、补充事实，以及对敏感问题的拒答信息。
> 输出：结构化 `PersonaProfile v2`、人读版个人说明书、可供其他 AI 直接加载的长文本画像，以及按需生成的机读 JSON。
> 版本：v3.5 RC（2026-03-13），基于 #009 第13轮审查修订。核心变化：单问制从失败红线降级为优先目标；AlignmentCheck 禁止「暂无」式礼貌总结；Lessons 无具体事件必须标 Insufficient。

请直接使用工作区源文件作为实际执行版本，发布时若需真正独立打包，再将源文件全文同步进此处。
