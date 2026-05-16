# 聊天摘要

> 最后同步时间：2026-05-16

## 上次讨论内容

- 仓库主题：**个人学术网站**（Jekyll Academic Pages），对标 davidlxu.github.io 风格改造。
- 本地路径：`~/Projects/myWebsite`（仓库根目录即网站根目录）；远程 https://github.com/hughhyang/hughhyang.github.io ，默认分支 **`master`**。
- 2026-05-16：从旧版多文件 `context/` 迁移到极简模板；`.cursorrules` 与 `context/` 放在 `myWebsite` 根目录（已去掉嵌套的 `hughhyang.github.io/` 与 `cursor-context-template/`）。

## 决策与结论

- 继续使用 **Academic Pages (Jekyll)**，不换框架。
- 导航：**Publications / Projects / Blog / CV / Talks**。
- 跨设备：离开设备写本摘要并 push；新设备 `git pull` 后读本文件续聊。

## 代码改动（迁移前已有）

- 首页 `_pages/about.md`：模板说明 → 个人主页骨架（中英文结构、占位符）。
- 导航、CV 页假数据清理；`_config.yml` 更新 description / bio 占位。
- 本次迁移：删除旧 `context/README.md`、`state.md`、`decisions.md`、`open_questions.md`；替换 `.cursorrules`；新增本文件。

## 当前状态

- 主页骨架已搭好，个人信息与论文条目多为占位/示例，待填写。
- 目录已扁平化：在 Cursor 中直接打开 `~/Projects/myWebsite` 即可（无需再进子文件夹）。

## 下一步

- 填写 `about.md` 真实个人信息（中英文简介、教育、经历、奖项）。
- 补充 `_config.yml` 中 author（邮箱、Scholar、头像等）。
- 清理/替换 `_publications/` 示例论文为真实条目；本地预览后 push。

## 未解决问题

- 是否需要中英文双语导航切换（EN / 中文），还是单页内中英分块？
- 头像和论文配图资源是否已准备好？
- 是否需要访客统计（Google Analytics 或其他）？
- Talks / Teaching 是否保留？导航有 Talks 但内容为示例数据。
