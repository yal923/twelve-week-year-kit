# WorkBuddy 独立验证交接

2026-09-20 最新收件：[NUM-01.1 单文件方案](../superpowers/plans/2026-09-20-workbuddy-number-check.md)对应的 numeric-diagnostic-summary.md 已收到。报告一次 ProbeValue 2→5 更新成功；本轮核对范围及待澄清项见[复测核对](../../reviews/workbuddy-numeric-retest-2026-09-20.md)。原值已改变，不重跑该方案或下面的旧整包，也不自动还原；如需补充执行证据，仅整理已有日志。

## 原始整包交接｜历史记录

这次交付的是 `workbuddy-capability-check-2026-09-19.zip`，用于首批两人内部能力试验，不是正式安装包。不要发送包含私人上下文的父工作目录，也无需发送整个开发仓库。

压缩包内容：START_HERE.md、AGENTS.md、CAPABILITY_PLAN.md、SCOPE_AND_RECOVERY.md、ISOLATED_PROBE_EXCEPTION.md、KNOWN_LIMITATIONS.md、REPORT_TEMPLATE.md、probe.sh、input.txt、MANIFEST.json。清单保留共同试验的固定输入、写入上限、日志和恢复要求；去除开发插件依赖。probe.sh 仅检查本地进程和文件，不连接 Notion。

1. 接收方在自己的 Mac 解压，让 WorkBuddy 打开整个目录。
2. 使用她自己的 Notion 连接，在自己的工作区准备空白测试页。
3. 复制 START_HERE.md 的启动文字，填写自己的页面链接并授权；运行、记录和比对由 Agent 执行，无需另写 plan 或输入终端命令。
4. 若遇内部重试证据不足，有限例外由该账号本人另行决定，不能继承开发者的授权。其他未解决缺口依然停止相关步骤。
5. 完成后只返回脱敏的 shareable-summary.md；真实账号、页面链接、映射、截图和原始回执保留在接收方包外私有目录。Agent 不自动发给开发者。

来源固定为工程设计提交 `a78649ab880e3cccbb188a5bb225453b325b6df0` 和[能力计划](../superpowers/plans/2026-09-19-minimal-capability-validation.md)提交 `225836352cceb7b950a3a95922cfeb48d788551e`。MANIFEST 记录包内逐文件 SHA-256；不包含开发者的运行配置或授权。该验证资料包不是已选择许可证的正式公开产品发布。

当前 Codex 的实测限制见[能力报告](../../reviews/capability-check-2026-09-19-codex.md)。WorkBuddy 版本、权限、接口与行为必须独立验证；两侧都使用 Mac 不能替代证据。
