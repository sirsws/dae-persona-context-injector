<!--
文件：README.zh-CN.md
核心功能：作为旧 DaE 公共仓的中文 README，明确它现在是 AKM 母港体系下的 DaE 分支公开入口。
输入：AKM 母定义、DaE 论文线、分发目标与当前分支级发布资产。
输出：适合旧 DaE 公共仓对外使用的中文总览页。
-->

# DaE：AKM 的首个参考实现

**先建画像，再做协作。**

[English](./README.md)

DaE 是 **主动知识建模（AKM）** 在 Persona / 顾问协作场景中的首个完整实现。

这个仓库现在应被理解为 AKM 生态中 `DaE 分支` 的历史公开入口，而不是 AKM 母概念本身的权威源头。

## DaE 做什么

DaE 把主动用户建模落成一个可直接使用的分支：先生成可复用的 `PersonaProfile`，再让下游智能体在规划、编码、写作、研究或顾问前先读档。

## DaE 在 AKM 结构中的位置

AKM 分三层：

- 母概念层
- 分支实现层
- 派生研究证据层

DaE 位于第二层。

## 研究基础

概念母源是 **AKM**，不是这个仓库。

DaE 的公开论文：

**Dialogue as Elicitation: A Framework for High-Fidelity Persona Profiling in Human-AI Collaboration**  
https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5961054

相关研究仓：

https://github.com/sirsws/DaE-Personal-Strategic-Asset

AKM 母港：

https://github.com/sirsws/akm

## 分支入口

- 当前母港分支页：https://github.com/sirsws/akm/tree/main/branches/dae
- 本仓内 skill 包：`./skills/dae-persona-context-injector/SKILL.md`
- benchmark 资产：`./benchmark/`

## 一句话概括

DaE 是 AKM 的首个完整分支实现：先把用户模型建出来，再让下游智能体从更强的起点开始工作。

