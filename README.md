# Twelve Week Year Kit

用共同的方法和引导流程，帮助不同使用者在各自的 Notion 中建立、执行和复盘 12 周计划。

**当前状态：规格审阅阶段，尚无可安装产品。禁止将本仓库的草案当作已经验证的运行流程。**

当前规格为 `0.1.0-review.4`：以两轮反馈修订后的 review.3 为基线，补充“说明书＋预写工具”、授权后全自动安装及跨 Agent 复现的工程设计。首批验证 Mac + Codex、Mac + WorkBuddy。[反馈记录](reviews/feedback-log.md)保留历次处置；既有报告针对旧提交，不能视为本版已经通过。

本项目借鉴 Brian P. Moran 与 Michael Lennington 的 *The 12 Week Year*（2013）。这是独立的产品设计，不代表作者或出版方的官方产品。仓库不包含书籍原文文件或真实使用者数据。

2026-09-19 已在获准隔离页面执行 Codex 最小能力试验：关系、视图、动态更新和小样例分页取得证据；标记与公式机器回读、内部重试等仍有缺口。[实测报告](reviews/capability-check-2026-09-19-codex.md)与 [WorkBuddy 交接说明](docs/testing/workbuddy-handoff.md)将已测和未测分开；这不等于完整安装通过。

2026-09-20 已收到 WorkBuddy 测试摘要，报告数字字段写入失败并阻断后续场景；根因待原始请求补证。[两端能力对照](reviews/capability-comparison-2026-09-20.md)保留不同证据等级，双宿主兼容尚未通过；下一步先只读补证，无需重跑整个包。

## 此次交付是什么

- 两份核心文档：方法蓝图与用户引导／复盘协议。
- 一份带需求编号、边界和验收依据的产品规格。
- 数据约定、Notion 落地候选、平台适配和分发架构。
- 自动搭建工程草案：共同结构、工具职责、交接接口与一致性验收；尚未交付完整可执行结构。
- 供独立 Agent／LLM 审核的任务说明与场景清单。

未来 v0.1 才会交付 ZIP 使用包，内含说明书和预先编写的小工具：使用者交给已有的 Codex 或 WorkBuddy，连接本人 Notion、指定位置并授权后自动搭建，无须手工配置字段或视图。这个自动化目标仍待实测；异常恢复保留安全暂停。日常数据保存在各自工作区，无需共享开发者账号或服务器。

## 阅读顺序

1. [阶段与授权](STATUS.md)、[Agent 约束](AGENTS.md)
2. [产品规格](docs/specs/v0.1-spec.md)
3. [方法蓝图](core/twelve-week-year-blueprint.md)、[引导与复盘协议](core/guidance-protocol.md)
4. [架构](docs/architecture.md)、[数据约定](docs/data-contract.md)、[搭建工程设计](docs/specs/notion-build-spec.md)
5. [决定与待验证项](docs/decisions.md)、[验收场景](checks/acceptance-scenarios.md)
6. [独立审核请求](reviews/REVIEW_REQUEST.md)

## 产品范围

首批范围是两位 Mac 使用者：一位使用 Codex，一位使用 WorkBuddy；两人各用自己的 Notion。共同流程包括开始周期、安排本周、复盘并恢复、周期交接。方法核心不随用户或平台改变；个人愿景、容量、目标和反馈属于个人数据。Codex 取得局部探针证据，WorkBuddy 摘要报告部分通过和明确阻断；最终工具运行包未验证，不宣称所有 Mac 均兼容。

初版不包含独立 App、集中托管、多用户后台、自动通知、后台监控或双向数据同步。不宣称周末内能够验证长期目标改善。

## 阶段顺序

需求细化 → spec 与架构 → GitHub 发布审阅材料 → 外部 Claude 审核 → 反馈处理与规格批准 → 实施计划批准 → 实现与试用。

GitHub 发布的是审阅材料，不是产品上线。外部审核通过也不自动授权实现；下一阶段以项目所有者明确决定和 [STATUS.md](STATUS.md) 为准。

## 如何审核

在 VPS 中读取 [REVIEW_REQUEST.md](reviews/REVIEW_REQUEST.md)，记录当前提交 SHA，再按指定维度审阅。无需提供作者的私人项目或原始书籍文件。未持有原著时，只能审查蓝图内部一致性和方案对蓝图的符合程度，不能声称完成原著准确性审校。

目前未选择开源许可证；公开的目的是审阅和讨论。许可证选择列入交付前决定，不把“公开可见”写成“已经完成开源授权”。
