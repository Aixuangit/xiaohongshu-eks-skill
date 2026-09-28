# xiaohongshu-ops：Codex 版

在 Codex 中协助小红书账号定位、页面研究、选题、原创图文创作、发布准备、评论回复与复盘。浏览器操作使用 Codex 当前可用的内置浏览器；用户指定 Chrome 时使用 Chrome。无需 OpenClaw、本地服务或固定浏览器 profile。

## 使用

在 Codex 中调用 `$xiaohongshu-ops`，例如：

- “分析这个账号最近的笔记，给出 5 个选题。”
- “研究这个链接的内容结构，写两版原创图文草稿。”
- “用我 Chrome 里已经打开的小红书页面检查最新评论。”
- “将这篇图文填入我的账号，先给我看最终预览。”

首次需要小红书登录时，用户在所选浏览器中自行扫码或处理验证码。若 Codex 当前环境无法操作所指定的 Chrome 标签页，skill 会说明限制并继续完成可离线处理的内容。发布和评论发送只在用户已明确授权具体内容后执行；提交结果不明时不会自动重发。

## 文件

- `SKILL.md`：任务路由、账号隔离和对外动作边界。
- `references/codex-browser.md`：Codex 内置浏览器与 Chrome 的选择及操作原则。
- `references/`：账号分析、研究、选题、创作、发布、评论和知识库流程。
- `persona.md`：当前账号语气资料，可由用户填写；`examples/xiashu-persona.md` 是原作者账号的可选示例。
- `knowledge-base/`：用户希望持续沉淀时可保存本地运营记录；运行记录默认不提交 Git。

改编自 [Xiangyu-CAS/xiaohongshu-ops-skill](https://github.com/Xiangyu-CAS/xiaohongshu-ops-skill)。本地改造以 Codex 工具能力为准，原仓库的 OpenClaw 安装说明不适用。

登录状态分端核验、参考资料到草稿的流程设计参考了 [cv-cat/XHS_ALL_IN_ONE](https://github.com/cv-cat/XHS_ALL_IN_ONE) 的产品结构；未复制其代码或素材。该项目 README 标明仅供学习交流。
