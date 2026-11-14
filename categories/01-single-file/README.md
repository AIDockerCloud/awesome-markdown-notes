# 单文件 Markdown 编辑器（Typora 式平替）— 分类清单

> 对应主清单：[根 README.md「单文件 Markdown 编辑器」](../../README.md)
> 本层定义：打开一个 `.md` 文件就写，所见即所得，不先建库、不先同步。

## 对比表

**本表即每周核实的对象清单**：新增软件只要在此登记一行，就会自动进入下一轮检查。

| 软件 | 一句话定位 | 协议 | 平台 | 数据真源 | AI 形态 | 详情 |
| --- | --- | --- | --- | --- | --- | --- |
| MarkText | 与 Typora 手感最接近的开源平替 | MIT，免费 | Win / macOS / Linux | 本地 `.md`，无账号无遥测 | 无内置 | [marktext.md](marktext.md) |
| Zettlr | 偏学术长文的写作工作台 | GPL-3.0，免费 | Win / macOS / Linux | 本地 `.md` | 无内置 | [zettlr.md](zettlr.md) |
| ghostwriter | KDE 无干扰写作，左右分栏预览 | GPL-3.0，免费 | Win / Linux | 本地 `.md` | —（未核实） | [ghostwriter.md](ghostwriter.md) |
| Aropyt | 自称「自由版 Typora」，编辑区即预览区 | AGPL-3.0，免费 | Win / macOS / Linux / Android | 本地 `.md` | 无内置 | [aropyt.md](aropyt.md) |
| TypeOpen | 轻量原生 macOS 实时编辑器 | Apache-2.0 | 仅 macOS（Apple Silicon） | 本地 `.md` | 无内置 | [typeopen.md](typeopen.md) |
| Tydora | 单文件编辑器：PDF 导出 / 页面背景 / 侧栏路径 | Apache-2.0 | —（未核实） | —（未核实） | —（未核实） | [tydora.md](tydora.md) |
| solomd | 单文件编辑器：打印 / 导出 / 中文 IME / WebDAV / 内置 AI | MIT | 桌面 + 移动（Tauri） | 本地 `.md` 文件夹 | 内置（MCP server + BYO-key AI 对话） | [solomd.md](solomd.md) |
| morrow | 测试预览阶段编辑器：Windows 预览包 / 主题插件 | AGPL-3.0 | 仅 Windows | 本地 `.md` | 无内置 | [morrow.md](morrow.md) |
| nomo | 单文件编辑器：折叠块 / Word 导出 / 自定义主题 | AGPL-3.0 | —（未核实） | 本地 `.md` | 无内置 | [nomo.md](nomo.md) |

> [已确认] 2026-11-10 由观察名单转入的后 4 款，经人类确认收录（DEC-006）。2026-11-14 首次联网核实已将 Tydora（Apache-2.0）、solomd（MIT / 本地 .md / 内置 AI）、morrow（AGPL-3.0 / Windows）、nomo（AGPL-3.0 / 本地 .md）四字段补实；「一句话定位」摘自旧任务历史报告，属 [推断]。

## 本类整体情况

- [事实] **数据真源**：9 款中 8 款已判定为本地 `.md`（MarkText、Zettlr、ghostwriter、Aropyt、TypeOpen、morrow、nomo、solomd），仅 Tydora 待核实。
- [事实] **AI 形态**：solomd 已判定为**内置 AI**（MCP server + BYO-key 对话）；MarkText、Zettlr、ghostwriter、Aropyt、TypeOpen、morrow、nomo 共 7 款明确无内置 AI；仅 Tydora 待核实。本层仍以「非 AI 卖点」为总体分界，solomd 的 AI 是个体例外。
- [事实] **协议**：MIT 2（MarkText、solomd）、GPL-3.0 2（Zettlr、ghostwriter）、AGPL-3.0 3（Aropyt、morrow、nomo）、Apache-2.0 2（TypeOpen、Tydora）；9 款全部已判定，均免费开源。
- [事实] **平台覆盖**：桌面三端 3 款（MarkText、Zettlr、ghostwriter）；TypeOpen 仅 macOS（Apple Silicon）；Aropyt 跨 Win / macOS / Linux / Android；solomd 桌面 + 移动（Tauri）；morrow 仅 Windows；nomo、Tydora 待核实。
- [事实] **手感并不统一**：ghostwriter 是左右分栏预览，与基准的「原地渲染、无分栏」不同。本层按「单文件本地 `.md`」宽口径归类，不是严格按手感对齐，选型时要单独看。
- [已确认] 2026-11-10 人类确认把 Tydora、solomd、morrow、nomo 由候选转入本类正表（DEC-006），四字段已于 2026-11-14 首轮核实补齐（Tydora 的平台 / 数据真源 / AI、nomo 的平台仍待进一步核实）；其中 morrow 只有测试预览版，已按人类确认保留正表（DEC-009）。
- [已确认] 2026-11-10 人类确认 **TypeOpen 保留在本类正表**，不转候选（DEC-007）；四字段未齐继续显式写「—（未核实）」，不猜测填充。
- [未决] 四字段齐全度 8/9：仅 Tydora 的平台 / 数据真源 / AI 三项、ghostwriter 的 AI 形态仍待进一步核实；nomo / morrow 个别字段已据软件形态判定（单文件编辑器 → 本地 .md）但平台待确认。
- [未决] 3 条链接锚定到 `develop` / `HEAD` 分支或具体 release tag，需去版本化。

## 边界与跨界指回

- 需要建 vault / 建库才能用 → [知识库与笔记系统](../03-knowledge-base/README.md)。
- 卖点是内置 AI 或 agent 共编 → [AI 与 Agent 时代的新编辑器](../02-ai-editors/README.md)。
- 本层 9 款均不进其它分区主表；同一软件只进一个主分区，避免双头维护。

## 进展（每周更新）

| 日期 | 软件 | 进展 | 来源 |
| --- | --- | --- | --- |
| 2026-11-10 | — | 分类清单与 5 张产品卡片初版建立 | 根 `README.md` |
| 2026-11-10 | MarkText | **历史回填（未联网复核）**：10-18 / 10-21 连发 v0.22.0（GitHub Alerts）与 v0.23.0（可折叠标题、独立大纲、只读阅读模式、Linux arm64），从长期半停滞恢复活跃；11-06 快照为 v0.24.0-rc.1 | 旧任务 `outbox/笔记软件开发进展_2026-10-23.md`、`snapshot_2026-11-06.json` |
| 2026-11-10 | Tydora / solomd / morrow / nomo | [已确认] 由候选观察名单转入本类正表（DEC-006），各建一张产品卡片并补入对比表；四字段全部 `—（未核实）`，归类依据为旧任务报告 [推断] | 用户 2026-11-10 指示 + [`../_WATCHLIST.md`](../_WATCHLIST.md) |
| 2026-11-10 | — | 定时任务改为每周六 09:00 运行，旧「笔记软件更新进展」任务已删除 | 用户 2026-11-10 指示 |
| 2026-11-14 | MarkText | 首次联网核实：v0.24.0-rc.2（预发布，11-13）；稳定版仍 v0.23.0；提交活跃（11-14） | GitHub API（marktext/marktext） |
| 2026-11-14 | Tydora | 发 v0.3.3（11-10）；GitHub API 确认协议 Apache-2.0 | GitHub API（zuorn/Tydora） |
| 2026-11-14 | solomd | 发 v5.0.21（11-12，9 天内 8 个补丁版）；四字段补实：MIT / 本地 .md / 内置 AI（MCP server + BYO-key） | GitHub API + solomd.app |
| 2026-11-14 | morrow | 仍只有测试预览版（0.1.9-test.56），无正式 Release；仓库 11-12 有零星提交未发版；协议 AGPL-3.0 确认 | GitHub API（StarrySky7D4/morrow） |
| 2026-11-14 | nomo | 发 v0.7.2（11-12）；协议 AGPL-3.0、数据真源 本地 .md 确认 | GitHub API（nomo-md/nomo） |
| 2026-11-14 | Aropyt | 首次联网核实：renxiaodaifu/aropyt（纠正原 Geekstrange 商店链接），~v0.1.9，AGPL-3.0，Win/mac/Linux/Android，本地 .md，无内置 AI；四字段全补实 | Microsoft Store + GitHub（renxiaodaifu/aropyt） |
| 2026-11-14 | TypeOpen | 首次联网核实：TriHerm/TypeOpen，Apache-2.0，仅 macOS（Apple Silicon），本地 .md，无内置 AI；最后活动 Oct 12 2026 | GitHub（TriHerm/TypeOpen） |

## 新增软件

1. 复制 [产品卡片模板](../_TEMPLATE.md) 到本目录，文件名用小写连字符；
2. 四字段判定不了写 `—（未核实）`，不要猜；
3. 在对比表补一行，链接指向新卡片；
4. 是否进主清单正表，由人类确认（见 [AGENTS.md](../../AGENTS.md)）。
