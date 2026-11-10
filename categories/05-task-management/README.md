# 任务管理 / Todo（自托管）— 分类清单

> 对应主清单：[根 README.md「任务管理 / Todo（自托管）」](../../README.md)
> 本节与笔记软件是两类东西：这里管的是任务本身，不是写笔记。收录它们的理由只有一个 —— 常被放在一起比较，但**任务到底存在哪里**完全不同，选错了等于选错了真源。

## 对比表

**本表即每周核实的对象清单**：新增软件只要在此登记一行，就会自动进入下一轮检查。

| 软件 | 一句话定位 | 协议 | 平台 | 数据真源 | AI 形态 | 详情 |
| --- | --- | --- | --- | --- | --- | --- |
| OpenTodo | 「你的任务、你的服务器」，小容器部署 | AGPL-3.0 | 自托管服务器 + 各设备离线副本 | **服务器** `/data` 卷里单个 SQLite（设备上是同步副本） | —（未核实） | [opentodo.md](opentodo.md) |
| TaskNotes | 一个任务 = vault 里一篇 Markdown 笔记 | —（未核实） | Obsidian 插件 | vault 内 `.md`（属性在 YAML frontmatter） | —（未核实） | [tasknotes.md](tasknotes.md) |
| taskquence | TaskNotes 衍生版，重时间统计仪表盘 | —（未核实） | Obsidian 插件 | vault 内笔记；time entry 在任务笔记、timeblock 在日记 frontmatter | —（未核实） | [taskquence.md](taskquence.md) |
| 思源 Task Horizon | 汇总思源文档里 checklist 的工作台 | —（未核实） | 思源内（依附知识库分区） | 原文档内的 checklist；工作台不另存数据 | —（未核实） | [siyuan-task-horizon.md](siyuan-task-horizon.md) |

## 任务真源对照（一眼看清选哪边）

| 项目 | 任务存在哪里 | 需要服务器吗 |
| --- | --- | --- |
| OpenTodo | 自托管服务器（SQLite），设备上是同步副本 | 需要，自托管 |
| TaskNotes / taskquence | Obsidian vault 内的 Markdown 笔记 | 不需要 |
| 思源 Task Horizon | 思源原文档内的 checklist，工作台只做汇总 | 不需要独立任务服务器 |

> 主清单推论：已经有一个任务真源时，不要再开第二个。OpenTodo 与 TaskNotes 可经 OpenTodo 的 vault 同步能力互相映射任务笔记，但**映射不等于双真源** —— 以哪边为准，要先定死。

## 本类整体情况

- [事实] **三种任务真源**：服务器 SQLite（OpenTodo）、vault 内笔记（TaskNotes / taskquence）、原文档 checklist（思源 Task Horizon）。只有 OpenTodo 需要服务器。
- [事实] **「视图」与「真源」是两件事**：TaskNotes 的看板 / 日历由 Obsidian Bases 查询笔记生成，思源 Task Horizon 只是汇总工作面，两者都不另存任务数据。
- [事实] Obsidian 的官方 OpenTodo 插件是把 Obsidian 当**操作入口**，任务仍存服务器，不会变成 vault 里的笔记文件 —— 与 TaskNotes 的模型正好相反。
- [事实] 四款 AI 形态全部未核实（4/4），是本类中信息缺口最集中的字段；协议也仅 OpenTodo 已判定。
- [未决] taskquence 主清单只给了 Obsidian Stats 条目页、未给独立仓库；思源 Task Horizon 未说明是内置还是插件。两者的「正式 Release + 近 6 个月提交」入选门槛都需补核实。

## 边界与跨界指回

- [Obsidian](../03-knowledge-base/obsidian.md) 与 [SiYuan](../03-knowledge-base/siyuan.md) 是这四款赖以运行的知识库底座，但主清单不因「笔记软件带了任务功能」就把它写成任务管理工具。
- 本分类单独成节，正是为了写清数据真源在哪一端。

## 进展（每周更新）

| 日期 | 软件 | 进展 | 来源 |
| --- | --- | --- | --- |
| 2026-11-10 | — | 分类清单与 4 张产品卡片初版建立 | 根 `README.md` |
| 2026-11-10 | — | 定时任务融合：融合进来的 16 款均为笔记 / 编辑器软件，本类无新增检查对象；「任务真源对照」口径不变 | [`../_WATCHLIST.md`](../_WATCHLIST.md) |

## 新增软件

1. 复制 [产品卡片模板](../_TEMPLATE.md) 到本目录，文件名用小写连字符；
2. 四字段判定不了写 `—（未核实）`，不要猜；**「数据真源」必须写清任务本体存在哪一端**；
3. 在对比表与「任务真源对照」补行，链接指向新卡片；
4. 是否进主清单正表，由人类确认（见 [AGENTS.md](../../AGENTS.md)）。
