# Awesome Markdown Notes — AI 时代的 Markdown 编辑器与笔记软件清单

> 仓库名：`awesome-markdown-notes`
>
> 本清单与 Typora 无关联，未获其背书或赞助。Typora 是其权利人的商标；本清单中提及 Typora，仅为指名性说明比较对象与判定基准。
>
> GitHub Topics 建议：`markdown`、`note-taking`、`awesome-list`、`ai`、`markdown-editor`

> AI 时代冒出来的新项目大多不在“排版更好”，而在 AI、MCP 和能不能被 agent 读写。这份清单按用途分层收录，不把单文件编辑器、知识库、速记和任务管理混在一张表里比。每条只记能判定的信息：协议、平台、文件存哪、AI 是内置还是插件；没有核实到的字段就不写。

## 目录

- [判定基准：Typora 本体](#判定基准typora-本体)
- [单文件 Markdown 编辑器（Typora 式平替）](#单文件-markdown-编辑器typora-式平替)
- [AI 与 Agent 时代的新编辑器](#ai-与-agent-时代的新编辑器)
- [知识库与笔记系统](#知识库与笔记系统)
- [速记与自托管笔记](#速记与自托管笔记)
- [任务管理 / Todo（自托管）](#任务管理--todo自托管)
- [已有的同类清单与目录](#已有的同类清单与目录)
- [收录标准与维护方式](#收录标准与维护方式)

## 判定基准：Typora 本体

- [Typora](https://typora.io/?from=MarkEditor) - 对照基准本身。单文件所见即所得：输入 Markdown 后格式直接在原地渲染，没有左右分栏预览。闭源，$14.99 一次买断、覆盖最多 3 台设备、15 天试用；Windows / macOS / Linux，无移动端；正文存本地 `.md` 文件；无内置 AI。

后面说“平替”时，先问平的是哪一点：是只要同样的所见即所得手感，还是要免费开源、要移动端、要 AI、还是要一整个知识库。答案不同，要看的分区也不同。

## 单文件 Markdown 编辑器（Typora 式平替）

这一层才是严格意义上的 Typora 平替：打开一个 `.md` 文件就写，所见即所得，不先建库、不先同步。

- [MarkText](https://raw.githubusercontent.com/marktext/marktext/develop/README.md) - 与 Typora 手感最接近的开源平替：单窗格实时渲染，底层仍是普通 `.md`。MIT，免费；Windows / macOS / Linux；本地 `.md` 文件，无账号、无遥测；无内置 AI。

- [Zettlr](https://github.com/Zettlr/Zettlr/releases/tag/v4.0.0-beta.1) - 偏学术与长文的写作工作台：实时预览之外主打引文（Zotero / BibTeX）、Zettelkasten 式链接和 Pandoc 导出。GPL-3.0，免费；Windows / macOS / Linux；本地 `.md` 文件；无内置 AI。

- [ghostwriter](https://github.com/kde/ghostwriter/blob/HEAD/README.md) - KDE 的无干扰写作编辑器，左右分栏预览，支持多种 Markdown 语法渲染与 Pandoc 导出。GPL-3.0，免费；Windows / Linux；本地 `.md` 文件。

- [Aropyt](https://github.com/Geekstrange/Aropyt) - 明确以“自由版 Typora”自居的新项目：编辑区即预览区，另加标签页、编辑历史、Vim 模式和插件系统。AGPL-3.0，免费；以 Windows 为主要构建目标，macOS / Linux / Android 同用 Tauri 2 外壳经 CI 构建。

- [TypeOpen](https://github.com/TriHerm/TypeOpen) - 轻量原生 macOS 编辑器，Typora 式实时编辑工作流，AppKit / WebKit 实现，可经 Homebrew 安装。仅 macOS（Apple Silicon）。

## AI 与 Agent 时代的新编辑器

这一层的卖点不是排版，而是 AI 怎么进来：内置对话、RAG 检索、MCP，或者干脆让 coding agent 与人共编同一批文件。

- [MarkFlowy](https://github.com/drl990114/MarkFlowy) - 自称 “The AI Markdown Editor”：Tauri 实现、体积小，源码 / 所见即所得多模式切换，内置 AI 支持 Copilot 式补全、翻译与摘要，可接 DeepSeek、ChatGPT 等模型。开源；Windows / macOS / Linux；本地文件。

- [NoteGen](https://github.com/codexu/note-gen) - “先捕获、后整理”：文字、语音、截图、文件先随手记下，再用 AI 整理成结构化 Markdown 笔记。GPL-3.0；桌面端 Windows / macOS / Linux（beta），移动端尚在 alpha；本地 Markdown 存储，可经 Git / WebDAV 同步；内置 AI 对话、摘要、OCR、知识库检索与 MCP 支持，需自备模型服务。

- [Nimbalyst](https://nimbalyst.com/app/) - 不是单纯的编辑器，而是给 coding agent 用的可视化工作台：在同一个窗口里跑 Claude Code、Codex 等 agent，人与 agent 共编 Markdown、图、原型和代码，agent 的改动以红绿 diff 呈现、逐块确认。桌面与 iOS 应用 MIT，个人免费；Windows / macOS / Linux；文件留在本地项目 / Git 仓库里。

- [Blinko](https://www.opentechhub.io/blinko/) - AI 优先的卡片速记（同时收录于下方速记分区）：自托管，靠 RAG 做自然语言找回旧笔记。GPL-3.0；数据存 PostgreSQL + pgvector；有托管云可选，但自托管才是它的主场。

## 知识库与笔记系统

这一层解决的是“笔记之间怎么连、怎么查”，不是单文件手感。把它们当 Typora 平替会错位：迁移成本、数据格式和日常操作完全是另一回事。

- [Obsidian](https://obsidian.md/help/official-site) - 本地文件夹（vault）之上的知识库：双向链接、图谱和庞大的社区插件生态。闭源，个人使用免费，Sync / Publish 为付费附加服务；Windows / macOS / Linux / iOS / Android；正文是 vault 内的 `.md` 文件；AI 靠社区插件接入。

- [SiYuan 思源笔记](https://github.com/siyuan-note/siyuan/releases/tag/v3.8.3) - 块级引用的个人知识管理：段落、标题、列表项都可被引用、嵌入、双向链接，并可用 SQL 查询；另有闪卡、数据库视图、PDF 标注。AGPL-3.0，核心免费、部分功能付费；Windows / macOS / Linux / iOS / Android，可自托管；数据存自有工作空间（可导入 `.md`，不是裸 `.md` 文件夹）；AI 写作与问答走 OpenAI 兼容接口。

- [Joplin](https://github.com/laurent22/joplin/blob/dev/readme/index.md) - 老牌开源笔记与待办：笔记本 + 标签组织，端到端加密同步。AGPL-3.0，免费，Joplin Cloud 付费；Windows / macOS / Linux / iOS / Android；笔记以 Markdown 形式组织，但存自有数据库，可导入 `.md` / Evernote 的 `.enex`。

- [Logseq](https://raw.githubusercontent.com/logseq/logseq/master/README.md) - 大纲式、块引用的知识管理，每天从日记页开始写。AGPL-3.0，免费；桌面 / Web / 移动端；文件版图谱存 Markdown / Org 文件，新数据库版改存 SQLite 且仍在 beta、官方提示有数据丢失可能，拿它当主力前先做好备份。

- [TriliumNext Notes](https://github.com/TriliumNext/Notes/releases/tag/v0.94.1) - 层级树状的大型个人知识库，原 Trilium 进入维护模式后由社区接续的版本，可无缝沿用原有数据库。开源；桌面端加可自托管的同步服务器；数据存自有数据库，不是裸 `.md` 文件夹。

- [SilverBullet](https://silverbullet.md/personal) - 可编程的自托管知识库：笔记是文件夹里的普通 Markdown，却能像数据库一样查询，还能在笔记里用 Space Lua 写逻辑。MIT；以浏览器 PWA 为主，可自托管；正文存普通 `.md` 文件夹。

- [AFFiNE](https://github.com/toeverything/AFFiNE) - 文档、无边白板与多视图数据库合一的工作台，本地优先、可自托管。协议按组件区分：客户端多为 MIT，部分后端 / 企业组件另有 MPL-2.0 与企业版条款，商用前需逐组件确认；不是纯 `.md` 存储。

- [HedgeDoc](https://github.com/hedgedoc/hedgedoc) - 实时协作的 Markdown 笔记（前身 CodiMD / HackMD CE）：多人同编、演示模式与图表渲染。AGPL-3.0；Web 应用，自托管部署；笔记存服务器数据库，强项是协作而不是个人知识库。

## 速记与自托管笔记

这一层比的是捕获速度：想到就记、时间线找回，不要求先想好标题、文件夹和结构。

- [memos](https://github.com/usememos/memos) - 时间线式的自托管速记：打开就写，Markdown 原生，单 Go 二进制或一个 Docker 容器即可跑。MIT，免费；自托管 Web 应用；数据存 SQLite（可换 MySQL / PostgreSQL）。

- [Blinko](https://www.opentechhub.io/blinko/) - AI 卡片速记，见上方 AI 分区。自托管、RAG 找回是它与 memos 拉开差距的两点；代价是部署更重（PostgreSQL + pgvector）。

- [flatnotes](https://raw.githubusercontent.com/dullage/flatnotes/develop/README.md) - 无数据库的自托管 Web 笔记：一整个平坦文件夹的 Markdown 文件，靠全文搜索、标签和双链组织，明确不设文件夹与笔记本层级。MIT；自托管 Web 应用；正文就是文件夹里的 `.md` 文件，随时可整体搬走换别的软件打开。

## 任务管理 / Todo（自托管）

这一节与上面的笔记软件是两类东西：这里管的是任务本身，不是写笔记。收录它们的理由只有一个——三者经常被放在一起比较，但**任务到底存在哪里**完全不同，选错了等于选错了真源。

- [OpenTodo](https://github.com/OpenTodoApp/OpenTodo) - 自托管任务管理应用，不是笔记编辑器。AGPL-3.0；“你的任务、你的服务器”：一个小容器即可部署，数据集中在一个 `/data` 卷里的单个 SQLite 文件中，服务器负责同步、备份与共享，各设备离线时保留完整副本、联网后再同步。官方 Obsidian 插件 obsidian-opentodo（OpenTodoApp/obsidian-opentodo）的定位是把 Obsidian 当作操作入口——在 Obsidian 里看和改任务，但**任务仍存 OpenTodo 服务器**，不会变成 vault 里的笔记文件。

- [TaskNotes](https://community.obsidian.md/plugins/tasknotes) - Obsidian 插件，模型与 OpenTodo 正好相反：**一个任务就是 vault 里的一篇 Markdown 笔记**，状态、优先级、到期日等写在 YAML frontmatter 里，列表、看板、日历等视图全部由 Obsidian Bases 查询这些笔记生成；没有插件专用数据库，也不需要任何服务器。

- taskquence（TaskNotes Time） - 基于开源 TaskNotes 发展出的 Obsidian 插件，底层模型与 TaskNotes 相同——任务仍是 vault 内的笔记；差别主要在时间维度：它在 time entry（向后看的实际用时记录，存在任务笔记的 frontmatter 里）的目标汇总与统计仪表盘上更重，timeblock（向前看的计划时间块，存在日记的 frontmatter 里）方面与 TaskNotes 基本无差别。可在 [Obsidian Stats 的 taskquence 页面](https://www.obsidianstats.com/plugins/taskquence) 查看其条目。

- 思源 Task Horizon - 思源里的任务工作台：它汇总散落在思源各文档里的 checklist，集中成一个工作面来查看和推进，但**任务本体仍留在原文档的 checklist 里**，工作台本身不另存一份任务数据。它依附于思源的知识库分区（见上方思源条目），不是独立的任务服务器。

三者的存储位置一句话分清：

| 项目 | 任务存在哪里 | 需要服务器吗 |
| --- | --- | --- |
| OpenTodo | 自托管服务器（SQLite），设备上是同步副本 | 需要，自托管 |
| TaskNotes / taskquence | Obsidian vault 内的 Markdown 笔记 | 不需要 |
| 思源 Task Horizon | 思源原文档内的 checklist，工作台只做汇总 | 不需要独立任务服务器 |

推论很直接：已经有一个任务真源时，不要再开第二个。OpenTodo 与 TaskNotes 可以经 OpenTodo 的 vault 同步能力互相映射任务笔记，但映射不等于双真源——以哪边为准，要先定死。

## 已有的同类清单与目录

现成清单不是没有，而是口径各异：有的只收编辑器，有的只收自托管，有的靠投票排序。下面这些值得直接当上游索引用，本清单与它们的关系是精选与分层，而不是替代。

### Awesome 与 GitHub 清单

- [Awesome Markdown](https://github.com/mundimark/awesome-markdown?utm_source=AAFREE) - Markdown 生态总清单：库、服务、编辑器、工具与速查表，编辑器只是其中一节，Typora 也收录在内。适合查“某个环节有什么工具”，不适合直接选笔记软件。

- [Awesome Markdown Editors & (Pre)viewers](https://github.com/mundimark/awesome-markdown-editors/blob/master/README.md) - 上一条的姊妹篇，专收 Markdown 编辑器与预览器，按在线 / 桌面 / 平台分节。与本清单编辑器分区重叠最多，适合当增补来源。

- [Awesome-Selfhosted 的 Note-taking & Editors 分节](https://github.com/awesome-selfhosted/awesome-selfhosted/blob/master/README.md) - 自托管口径的笔记与编辑器清单，Blinko、flatnotes、HedgeDoc、Joplin 等都在其中，每条带协议与部署标签。只收能自托管的自由软件，桌面单机编辑器不在其内。

- [appsgit 的开源笔记与写作应用目录](https://appsgit.com/desktop-apps/category/notes-writing) - 按 GitHub 星数排的桌面开源应用目录（该分类 57 款），每条带平台、协议与安装命令，并有明确的入选门槛（如近半年有提交、非 fork）。适合按热度与活跃度筛粗选名单。

### 目录站与投票型站点

- [Markdown Editors 目录](https://www.markdowneditors.com/) - 纯编辑器口径的目录站：Markdown 编辑器、笔记应用、代码与文本编辑器分开计数与陈列，条目带原生 / Electron、付费 / 免费、开源 / 闭源标签。

- [AlternativeTo 的 Typora 条目](https://alternativeto.net/software/typora/about/) - 投票型替代品目录，Typora 名下挂着两百多个替代品。优点是全，缺点是编辑器、知识库、速记混排且排序靠用户投票，只能当线索池，不能当结论。

- [Product Hunt 的 Typora 竞品页](https://www.producthunt.com/products/typora/alternatives) - 以产品发布口径整理的 Typora 替代品，适合发现新面孔，深度与维护信息都有限。

### 测评与对比文章

- [Markdific：14 Best Typora Alternatives (2026), Tested and Compared](https://markdific.com/blog/typora-alternatives/) - 逐款实测的对比文，表格列了价格、协议、平台与文件存储方式，是少数把“文件存成什么”写进对比的文章。注意它自家产品也在榜内，结论需打折看。

- [Nimbalyst：Typora Alternatives 2026 — Open Source Markdown Editors](https://nimbalyst.com/blog/typora-alternatives-2026/) - 从“Typora 闭源、无 AI、单文件在工作流之外”三个动机出发选品，AI 一栏写得最实；同样自带自家产品，立场需注意。

## 收录标准与维护方式

清单的价值在持续验活，不在一次收全。建议按下面几条维护：

- 有正式 Release，且近 6 个月内有提交；纯 fork、已归档、无 Release 的概念项目不收。
- 每条至少能判定四件事：协议、平台、数据存哪（裸 `.md` / 自有数据库 / 服务器）、AI 形态（内置 / 插件 / MCP / 无）。判定不了的项目先放候选，不进正表。
- 同一软件只进一个主分区，跨界的在另一分区一句话指回主条目，不重复写两份介绍——双头维护必然分叉。
- 每次更新只做两件事：新增通过门槛的项目，以及把停更、归档、改协议的旧条目标注或移出。价格与版本变化快，正文里只写不易过期的结构性信息，价格以官网为准。
- 任务管理、速记这类相邻品类单独成节，并写清数据真源在哪一端；不因为某个笔记软件带了任务功能，就把它写成任务管理工具，反之亦然。
- 仓库在 GitHub 上以 `awesome-markdown-notes` 维护，Topics 使用 `markdown`、`note-taking`、`awesome-list`、`ai`、`markdown-editor`，不以任何单一产品名作为仓库名或主 Topic；正文中对具体产品的提及均为指名性比较，不暗示官方关联或背书。
