# 来源与证据范围

整理日期：2026-09-19。来源帮助解释方法或技术设计，不替代实际兼容性测试。本文不包含书籍文件、私人路径、私人页面和登录凭证。

## 方法来源

Brian P. Moran、Michael Lennington，*The 12 Week Year: Get More Done in 12 Weeks than Others Do in 12 Months*，Wiley，2013，ISBN 9781118616420。英文正文与关键图例的阅读范围、中文重点对照限制以及章节对应见[方法蓝图](core/twelve-week-year-blueprint.md) B12。

方法蓝图为归纳和解释；引导问题和验收例子为本项目原创。原著中的作者经验、案例效果和 85% 参考线未被本项目独立实证验证，不承诺对所有使用者有效。社交媒体经验不作为 v0.1 方法或评分规则的权威依据；本阶段未形成可公开复用的系统性社交媒体证据集。

## 技术依据

| 官方来源 | 支持的设计判断 | 不支持的推断 |
|---|---|---|
| [Notion MCP supported tools](https://developers.notion.com/guides/mcp/mcp-supported-tools) | Notion 提供页面／数据库等工具能力，可据此建立安装能力检查 | 任意宿主、账户权限和工具版本都具备同样功能；本项目已经实测 |
| [Notion relations and rollups](https://www.notion.com/help/relations-and-rollups) | 关系适合表达关联；CSV 导出关系不能直接当作关系完整恢复方案 | 普通 CSV 来回导入即可无损克隆独立实例 |
| [WorkBuddy Skill 文档](https://open.workbuddy.cn/en/docs/skill) | 可用 SKILL.md 及辅助资料组织技能；可考虑薄入口 | 普通文件包必然全自动安装；各平台 frontmatter 和权限完全一致 |
| [WorkBuddy Skills Market 文档](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Skills-Market) | 宿主提供技能使用／管理入口，交付可适配其流程 | 已安装该技能、已验证目标用户设备与 Notion 连接 |
| [Agent Skills specification](https://agentskills.io/specification) | 核心指令与按需读取的辅助文件可以分层 | Skill 标准能统一所有 MCP 名称、权限和工具调用方式 |

上述资料在设计准备阶段查阅；网页与能力可能变化。实现前按实际宿主和连接再次检查，仅引用已读到的行为。文档未覆盖的 API 参数、字段限制、分页与幂等能力必须通过技术验证确定，不能凭概念设计推定。

## 开发方法

本次细化使用 Superpowers 的 brainstorming 工作流：先核对范围和上下文，比较方案，区分确认与假设，形成可审核规格。完成声明采用 verification-before-completion 的证据要求。没有因使用插件而自动进入实施计划或产品开发。

Superpowers 组织设计与验证过程，不是 12 Week Year 的方法来源，也不是运行时必须依赖的组件。未来使用者不需要安装它才能使用本产品。
