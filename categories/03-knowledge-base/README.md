# 知识库与笔记系统 — 分类清单

> 对应主清单：[根 README.md「知识库与笔记系统」](../../README.md)
> 本层解决的是「笔记之间怎么连、怎么查」，不是单文件手感；把它们当 Typora 平替会错位。

## 对比表

**本表即每周核实的对象清单**：新增软件只要在此登记一行，就会自动进入下一轮检查。

| 软件 | 一句话定位 | 协议 | 平台 | 数据真源 | AI 形态 | 详情 |
| --- | --- | --- | --- | --- | --- | --- |
| Obsidian | vault 之上的双链 / 图谱 / 插件生态 | 闭源，个人免费；Sync / Publish 付费 | Win / mac / Linux / iOS / Android | vault 内 `.md` | 社区插件 | [obsidian.md](obsidian.md) |
| SiYuan 思源 | 块级引用 + SQL 查询的知识管理 | AGPL-3.0，核心免费 | Win / mac / Linux / iOS / Android，可自托管 | 自有工作空间（非裸 `.md`） | OpenAI 兼容接口 | [siyuan.md](siyuan.md) |
| Joplin | 笔记本 + 标签，E2E 加密同步 | AGPL-3.0；Cloud 付费 | Win / mac / Linux / iOS / Android | 自有数据库 | —（未核实） | [joplin.md](joplin.md) |
| Logseq | 大纲式块引用，从日记页开始 | AGPL-3.0，免费 | 桌面 / Web / 移动端 | **分版本**：文件版 Markdown / Org；新数据库版 SQLite（beta，官方提示有数据丢失可能） | —（未核实） | [logseq.md](logseq.md) |
| TriliumNext | 层级树状大型个人知识库 | 开源（协议未写） | 桌面 + 可自托管同步服务器 | 自有数据库（非裸 `.md`） | —（未核实） | [triliumnext.md](triliumnext.md) |
| SilverBullet | 可编程知识库，Space Lua 写逻辑 | MIT | 浏览器 PWA 为主，可自托管 | 普通 `.md` 文件夹 | —（未核实） | [silverbullet.md](silverbullet.md) |
| AFFiNE | 文档 + 白板 + 多视图数据库 | **按组件**：客户端多 MIT，部分后端 / 企业组件 MPL-2.0 与企业版 | —（未核实） | 不是纯 `.md`（格式未写） | —（未核实） | [affine.md](affine.md) |
| HedgeDoc | 实时协作 Markdown（前身 CodiMD） | AGPL-3.0 | Web，自托管 | 服务器数据库 | —（未核实） | [hedgedoc.md](hedgedoc.md) |
| 虎鲸笔记 orca-note | 块式笔记：计算属性 / 日历视图 / 内置命令型 AI 助手 | —（未核实） | —（未核实） | —（未核实） | —（未核实） | [orca-note.md](orca-note.md) |
| Anytype | 对象 / 关系网络组织的本地优先知识库 | —（未核实） | —（未核实） | —（未核实） | —（未核实） | [anytype.md](anytype.md) |
| edgeever | 知识库 + 一键发布站点 + 多平台剪藏 + 内置 AI | —（未核实） | —（未核实） | —（未核实） | —（未核实） | [edgeever.md](edgeever.md) |
| tolaria | vault + 多端架构（远程后端 / 服务端搜索 / SSE） | —（未核实） | —（未核实） | —（未核实） | —（未核实） | [tolaria.md](tolaria.md) |

> [已确认] 2026-11-10 由观察名单转入的后 4 款，经人类确认收录（DEC-006）。四字段全部未判定，按硬约束 10 写 `—（未核实）`，不猜测填充；「一句话定位」摘自旧任务历史报告，属 [推断]，不是已核实的四字段事实。tolaria 因明确有 vault / 同步 / 服务端索引，归本层而非单文件层。

## 本类整体情况

- [事实] **数据真源是最大分水岭**：原 8 款中，裸 `.md` 2 款（Obsidian vault、SilverBullet）；自有工作空间 1（SiYuan）；自有数据库 2（Joplin、TriliumNext）；分版本 1（Logseq）；服务器数据库 1（HedgeDoc）；AFFiNE 判定为「非纯 `.md`」但具体格式未核实。本轮转入的 4 款全部未核实，12 款中已有判定的仍是 8 款。
  - 裸 `.md` 意味着可整体搬走换别的软件打开；数据库型需要显式导出 / 迁移。
  - Joplin 尤其要注意：「笔记以 Markdown 形式组织」说的是语法，不是存储格式。
- [事实] **AI 形态 10/12 未核实**；已判定的 2 款分别是社区插件（Obsidian）与 OpenAI 兼容接口（SiYuan），都不是内置模型。这是本类当前最大的信息缺口。
- [事实] **组织范式各不相同**：双链图谱（Obsidian）、块引用（SiYuan、Logseq）、层级树（TriliumNext）、平坦文件夹 + 可编程查询（SilverBullet）、多视图工作台（AFFiNE）、实时协作（HedgeDoc）、对象 / 关系网络（Anytype）、块式 + 计算属性（虎鲸笔记）、知识库 + 对外发布（edgeever）、vault + 多端同步（tolaria）。
- [事实] **协议不都是单一值**：AFFiNE 需逐组件确认，商用前尤其要核对；TriliumNext 只写了「开源」未给协议名。
- [事实] **显式风险项**：主清单对 Logseq 数据库版保留了官方的数据丢失风险提示，并建议当主力前先备份。
- [已确认] 2026-11-10 人类确认把虎鲸笔记、Anytype、edgeever、tolaria 由候选转入本类正表（DEC-006），四字段待首轮联网核实补齐；edgeever 的 1.x → 2.0 破坏性变更、tolaria 仅 Alpha 构建，均为重点复核项。
- [未决] 3 条链接锚定到具体 release tag 或 `dev` 分支 README，需去版本化。
- [未决] Logseq 数据库版若脱离 beta，「数据真源」一栏需整体改判，是每周核实的重点观察项。

## 边界与跨界指回

- 只写单个 `.md`、不建库 → [单文件 Markdown 编辑器](../01-single-file/README.md)。
- 想到就记、时间线找回 → [速记与自托管笔记](../04-quick-notes/README.md)。
- 任务真源相关：Obsidian 的官方 OpenTodo 插件把 Obsidian 当入口但 [任务仍存服务器](../05-task-management/opentodo.md)；[TaskNotes](../05-task-management/tasknotes.md) 反过来把任务存成 vault 笔记；[思源 Task Horizon](../05-task-management/siyuan-task-horizon.md) 汇总本类原文档里的 checklist。选型前先定死哪边是真源。

## 进展（每周更新）

| 日期 | 软件 | 进展 | 来源 |
| --- | --- | --- | --- |
| 2026-11-10 | — | 分类清单与 8 张产品卡片初版建立 | 根 `README.md` |
| 2026-11-10 | Obsidian | **历史回填（未联网复核）**：10-22 发 1.14.5（纯 Electron 安全补丁 43.7.5 → 43.8.3），11-02 发 1.15.0 | 旧任务 `outbox/笔记软件开发进展_2026-10-23.md`、`snapshot_2026-11-06.json` |
| 2026-11-10 | Logseq / TriliumNext | **历史回填（未联网复核）**：Logseq 主线转 DB 版同步可靠性加固、Beta 仍 2.0.2；TriliumNext Web Clipper 首次独立发版，主程序到 v0.106.1，v0.107.0 仍未发 | 同上 |
| 2026-11-10 | 虎鲸笔记 / Anytype / edgeever / tolaria | [已确认] 由候选观察名单转入本类正表（DEC-006），各建一张产品卡片并补入对比表；tolaria 归类定为知识库层；四字段全部 `—（未核实）` | 用户 2026-11-10 指示 + [`../_WATCHLIST.md`](../_WATCHLIST.md) |
| 2026-11-10 | — | 定时任务改为每周六 09:00 运行，旧「笔记软件更新进展」任务已删除 | 用户 2026-11-10 指示 |

## 新增软件

1. 复制 [产品卡片模板](../_TEMPLATE.md) 到本目录，文件名用小写连字符；
2. 四字段判定不了写 `—（未核实）`，不要猜；「数据真源」要写清是裸 `.md` / 自有工作空间 / 自有数据库 / 服务器；
3. 在对比表补一行，链接指向新卡片；
4. 是否进主清单正表，由人类确认（见 [AGENTS.md](../../AGENTS.md)）。
