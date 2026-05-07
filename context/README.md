# 项目上下文：个人学术网站

本仓库只服务一个主题：`个人学术网站`。

**本文件是会话流程与提示词的单一事实来源。**

## 核心文件
- `context/state.md`：当前状态与下一步行动。
- `context/decisions.md`：已确认决策（含日期与理由）。
- `context/open_questions.md`：未决问题与跟进项。
- `context/sessions/`：会话压缩摘要。

## 超短口令
会话开始、结束只用下面两条即可（不必再贴长段提示词）。

- `开始同步`：先按下面「开始同步时的 Git」在仓库根目录尝试 `git pull`，再读取 `context/README.md`、`context/state.md`、`context/open_questions.md`，用 3 句中文回复当前状态、下一步、最重要未决问题，然后等待指令。
- `结束归档`：把本次讨论压缩写入 `context/sessions/YYYY-MM-DD-个人学术网站.md`，并同步更新 `context/state.md`、`context/decisions.md`、`context/open_questions.md`，最后用 3 行总结结论/下一步/未决问题；然后按下面「结束归档后的 Git」约定提交并推送。

### 开始同步时的 Git（约定）
在仓库根目录对当前分支执行 `git pull`（对齐跟踪远程），**再**读 `context/`。电脑端本地克隆应能常规完成此步。若在已确认**无需** pull 的环境（例如部分手机端工作区），该命令可能不适用或失败，则**跳过** pull，直接读 `context/` 并继续；三句回复中用**一句**说明本次是否已成功 `pull`（或跳过原因）。

### 结束归档后的 Git（约定）
查看 `git status`，将**本次为归档而改动**的已跟踪文件纳入一次提交（通常集中在 `context/`；若本会话内还改过与项目约定相关的其他已跟踪文件且与归档一致，可一并纳入），写简短中文 commit message，执行 `git commit` 与 `git push` 到当前分支的跟踪远程，便于跨设备 `git pull`。不要把明显无关的本地改动混进该提交；若无法安全区分，则只提交 `context/` 并在收尾中提醒处理其余文件。若推送失败（凭据、网络、非快进等），在收尾中说明原因与建议操作。
