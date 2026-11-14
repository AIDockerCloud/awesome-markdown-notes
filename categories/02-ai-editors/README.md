# AI 与 Agent 时代的新编辑器 — 分类清单

> 对应主清单：[根 README.md「AI 与 Agent 时代的新编辑器」](../../README.md)
> 本层卖点不是排版，而是 AI 怎么进来：内置对话、RAG 检索、MCP，或者让 coding agent 与人共编同一批文件。

## 对比表

**本表即每周核实的对象清单**：新增软件只要在此登记一行，就会自动进入下一轮检查。

| 软件 | 一句话定位 | 协议 | 平台 | 数据真源 | AI 形态 | 详情 |
| --- | --- | --- | --- | --- | --- | --- |
| MarkFlowy | 自称 "The AI Markdown Editor"，Tauri 多模式 | AGPL-3.0 | Win / macOS / Linux | 本地文件 | **内置**：补全 / 翻译 / 摘要，可接 DeepSeek、ChatGPT | [markflowy.md](markflowy.md) |
| NoteGen | 先捕获、后整理，AI 生成结构化笔记 | GPL-3.0 | 桌面 Win / mac / Linux（beta）；移动端 alpha | 本地 Markdown，可 Git / WebDAV 同步 | **内置**：对话 / 摘要 / OCR / 知识库检索 / MCP | [notegen.md](notegen.md) |
| Nimbalyst | 给 coding agent 用的可视化工作台 | 桌面与 iOS 应用 MIT，个人免费 | Win / macOS / Linux | 本地项目 / Git 仓库 | **agent 工作台**：跑 Claude Code、Codex，红绿 diff 逐块确认 | [nimbalyst.md](nimbalyst.md) |

> 跨界指回：[Blinko](../04-quick-notes/blinko.md) 在主清单本分区也有一句话提及，但**主条目在速记层**；按「同一软件只进一个主分区」口径，此处不重复介绍。

## 本类整体情况

- [事实] **AI 形态是本层的分层依据**：3 款全部有 AI，且形态各不相同 —— 内置对话 / 补全 2 款、agent 宿主工作台 1 款；没有一款是「靠社区插件接入」。
- [事实] **数据真源全部在本地侧**：本地文件 2 款、本地项目 / Git 仓库 1 款；没有服务器数据库型。
- [事实] **成熟度差异**：NoteGen 桌面 beta、移动端 alpha；MarkFlowy 与 Nimbalyst 主清单未标注 beta。
- [事实] **MCP / agent 可读性**：NoteGen 明确写 MCP 支持，Nimbalyst 直接把 agent 当共同编辑者 —— 这两条最贴近主清单「AI 时代的新项目能不能被 agent 读写」的判断视角。
- [事实] 主清单同时收录了两篇带自家产品的测评文（见 [参考资料](../06-references/README.md)），其中一篇出自 Nimbalyst；引用时须保留「立场需注意」的折扣提示。
- [未决] MarkFlowy 的具体开源协议、Nimbalyst 的 MIT 覆盖组件范围，均需核实。
- [未决] NoteGen 的 beta / alpha 是否转为正式 Release，直接关系入选门槛。

## 边界与跨界指回

- 只求单文件编辑手感、无 AI → [单文件 Markdown 编辑器](../01-single-file/README.md)。
- 以速记捕获 + RAG 找回为主 → [速记与自托管笔记](../04-quick-notes/README.md)。
- 本层与单文件层的分界是「AI 是不是主卖点」，不是「数据存哪」—— 两者真源都在本地。

## 进展（每周更新）

| 日期 | 软件 | 进展 | 来源 |
| --- | --- | --- | --- |
| 2026-11-10 | — | 分类清单与 3 张产品卡片初版建立 | 根 `README.md` |
| 2026-11-10 | NoteGen | **历史回填（未联网复核）**：10-18 发 v0.38.3（桌面端 12 种代码块预览插件按需安装、AI 对话可引用笔记文件夹），10-23 起恢复连续提交；11-06 快照为 v0.39.2 | 旧任务 `outbox/笔记软件开发进展_2026-10-23.md`、`snapshot_2026-11-06.json` |
| 2026-11-10 | — | [已确认] 归类定了：edgeever、tolaria 按「自托管实例 / vault + 同步」归 [知识库层](../03-knowledge-base/README.md)，不进本类正表 | 用户 2026-11-10 指示 + `../_WATCHLIST.md` |
| 2026-11-14 | NoteGen | 首次联网核实：v0.39.2（11-01）无新发版（提交至 11-11） | GitHub API（codexu/note-gen） |
| 2026-11-14 | MarkFlowy | 首次联网核实：v1.3.0（11-07）；协议「开源（未写）」→ AGPL-3.0 已确认 | GitHub（drl990114/MarkFlowy） |

## 新增软件

1. 复制 [产品卡片模板](../_TEMPLATE.md) 到本目录，文件名用小写连字符；
2. 四字段判定不了写 `—（未核实）`，不要猜；AI 形态要写清是内置 / 插件 / MCP / agent 工作台 / RAG / 无；
3. 在对比表补一行，链接指向新卡片；
4. 是否进主清单正表，由人类确认（见 [AGENTS.md](../../AGENTS.md)）。
