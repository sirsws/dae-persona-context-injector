<!--
File: README.zh-CN.md
Core: Chinese companion README for the DaE product repository.
Input: English product positioning and the current release assets.
Output: Chinese overview page linked from the main README.
-->

# DaE：人格上下文注入层

**先建档，再协作。**

[English README](./README.md)

DaE 是面向智能体时代的上游上下文层。

它通过结构化追问生成可复用的 `PersonaProfile`，让下游智能体在开始规划、编码、写作、研究或给建议之前，先理解自己究竟在为谁工作。

## DaE 解决什么问题

绝大多数 AI 工作流失败，原因都一样：

**模型在理解用户之前就开始行动。**

于是用户重复解释，智能体靠猜，输出越来越像平均正确的废话。

DaE 的作用，就是先建一份可复用档案，再让后续智能体读取这份档案。

## DaE 做什么

DaE 只做三件事：

1. 通过结构化追问挖出高保真的人物画像
2. 生成可复用的 `PersonaProfile`
3. 让下游智能体先读档，再开工

DaE 不是：

- 心理疗愈机器人
- 一次性人格测试
- 普通 prompt 小技巧
- 直接给答案的人生导师

DaE 是：

- 可复用档案生成器
- 上游上下文注入层
- 面向下游协作的协议

## 为什么它不一样

DaE 不会把自我描述原样照单全收。

它会主动：

- 质疑空泛标签
- 强迫落到具体事件
- 用真实取舍校验宣称价值
- 输出张力、决策风格与约束逻辑

它产出的不是一份好看的总结，而是一份可复用的运行档案。

## 公开 benchmark

公开演示不会使用真实私人画像。

首个 benchmark 选用 **Steve Jobs** 作为公开历史对象，在同一个模型、同一个问题下，只改变是否加载 `PersonaProfile`：

- 无 PersonaProfile
- 加载 DaE PersonaProfile

测试问题：

**How should Steve Jobs rebuild Apple after returning to the company?**

详细内容见：

- [Benchmark 展示页](./benchmark/Steve-Jobs.md)
- [Benchmark PersonaProfile](./benchmark/Steve-Jobs-profile.md)

## 研究溯源

DaE 的研究基础来自论文：

**Dialogue as Elicitation: A Framework for High-Fidelity Persona Profiling in Human-AI Collaboration**  
https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5961054

对应研究仓库：

https://github.com/sirsws/DaE-Personal-Strategic-Asset

本仓库承载的是产品化发布资产与协议入口；论文仓库继续承担方法论与学术溯源职责。

## 产出结构

一份有效的 DaE 档案通常包含：

- `Background`
- `Capabilities`
- `Resources`
- `Constraints`
- `Drives`
- `Goals`
- `DecisionStyle`
- `Weaknesses`
- `Tensions`
- `Lessons`
- `AlignmentCheck`

这是一份配置资产，不是鸡汤文本。

## 分发形态

DaE 当前面向三类分发：

- `ClawHub / OpenClaw` 技能
- 智能体商店 onboarding agent
- 自定义 agent 工作流中的前置协议

当前文案草案见：

- [ClawHub 技能页文案](./docs/clawhub-copy.md)
- [智能体商店首屏文案](./docs/agent-store-copy.md)

## 边界与安全

- DaE 不替用户做最终决策
- DaE 不把人物档案伪装成行动方案
- DaE 不把人格标签当作证据
- 公开演示只使用非敏感 benchmark 对象
- 真实用户档案应被视为本地私有配置资产

## 当前状态

- 定位已收束
- 第一轮 benchmark 已完成
- ClawHub / GitHub / 智能体商店发布资产已备齐
- 待平台提交与安全测试
