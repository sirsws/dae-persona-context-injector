---
name: "dae-persona-context-injector"
description: "DaE 是 AKM 在 Persona 感知协作场景中的首个完整实现，在下游任务开始前先构建可复用画像。"
---

<!--
文件：SKILL.zh-CN.md
核心功能：作为旧 DaE 公共 skill 包的中文落地页，与 AKM 母港结构保持一致。
输入：AKM 母定义、DaE 分支角色、PersonaProfile 字段与当前公开发布用途。
输出：适合旧 DaE 公共仓使用的中文 skill 文档。
-->

# DaE Persona Context Injector

<p align="center">
  <a href="./SKILL.md">English</a> | <a href="./SKILL.zh-CN.md">简体中文</a>
</p>

DaE 是 **主动知识建模（AKM）** 在 Persona / 顾问协作场景中的首个完整实现。

这个公开 skill 包现在应被理解为 AKM 母港结构下的历史分支分发资产，而不是 AKM 母概念本身的权威源头。

## 快速说明

| 项目 | 内容 |
| --- | --- |
| 母概念 | `Active Knowledge Modeling (AKM)` |
| 生态角色 | `first branch implementation` |
| 主要产物 | 可复用 `PersonaProfile` |
| 最适用场景 | 下游智能体因缺少操作者画像而持续泛化回答 |
| 母港 | `https://github.com/sirsws/akm` |
| 当前分支页 | `https://github.com/sirsws/akm/tree/main/branches/dae` |
| 研究论文 | `https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5961054` |

## 核心规则

**先建画像，再做协作。**

## 源头层级

- 概念母源：上游 `AKM.md`
- 分支实现源：AKM 母港 + DaE 分支包
- 历史公开分发源：本仓
- 派生研究证据：SSRN 论文与研究仓

