# 巡检观察名单 (_WATCHLIST)

> 最近更新：2026-11-14 · 状态：[已确认] 16 款全部经人类确认转入正表
> 用途：**每周巡检对象的第二真源**，与 `categories/*/README.md` 的对比表并列。定时任务同时遍历两处，不依赖写死在任务提示词里的名单。
> 来源：旧任务「笔记软件更新进展」（每周五 18:00，2026-10-07 起运行 5 次），2026-11-10 融合进项目任务（每周六 09:00）后已删除。

## 使用口径

- [事实] 表内每一行都是本周要核实的对象，核实结论写入根 `CHANGELOG.md`，并更新本文件「上次快照」列。
- [已确认] 2026-11-10 原 8 款候选全部经人类确认转入正表，已建产品卡片、补入分类对比表与主清单；四字段未判定者一律写 `—（未核实）`，不猜测填充（DEC-006）。
- [事实] 后续若有新对象，可先记为「候选」只记录进展；是否升级为收录由人类确认，规则见 [AGENTS.md](../AGENTS.md)。
- [事实] 「上次快照」于 2026-11-14 **首次真正联网核实**后覆盖为当日结果（GitHub API / typoraio.cn）；此前一版为 2026-11-06 历史回填基线（来源 `data/snapshot_2026-11-06.json`）。每周任务核实后覆盖此列。
- [事实] 本文件只登记对象与基线，不写价格、不写主观评价；详细进展与来源写在 `CHANGELOG.md` 与产品卡片。
- [事实] `06-references` 的外部索引资源不在此表内，仍按分类清单单独核实链接可达性与口径变化。

## 巡检对象（16 款，均已收录）

| 软件 | 上游地址 | 主条目 | 分类 | 上次快照（2026-11-14） | 备注 |
| --- | --- | --- | --- | --- | --- |
| Typora | [官方发布页](https://typora.io/releases/stable.html) | [00-baseline/typora.md](00-baseline/typora.md) | 00-baseline | 1.14.15 稳定（11-14，typoraio.cn） | 闭源，无公开仓库；[已确认] 活跃度按官网发布记录判定（DEC-007）；`typora.io` DNS 异常时走官方中文站同页 |
| Obsidian | [obsidianmd/obsidian-releases](https://github.com/obsidianmd/obsidian-releases) | [03-knowledge-base/obsidian.md](03-knowledge-base/obsidian.md) | 03-knowledge-base | 1.15.1（11-12） | 闭源，用发布镜像仓库与官方 changelog 核实 |
| 虎鲸笔记 orca-note | [sethyuan/orca-note](https://github.com/sethyuan/orca-note) | [03-knowledge-base/orca-note.md](03-knowledge-base/orca-note.md) | 03-knowledge-base | 1.100.1（11-14），公开仓库仍只发 Release | 闭源（用户 2026-11-14 确认），按 DEC-007 以 Release 判定活跃度；AI 形态内置命令型 |
| Anytype | [anyproto/anytype-ts](https://github.com/anyproto/anytype-ts) | [03-knowledge-base/anytype.md](03-knowledge-base/anytype.md) | 03-knowledge-base | v0.57.8-alpha（11-10），提交 11-10 | 数据真源本地优先；开源（自定义许可 NOASSERTION，用户 2026-11-14 确认按开源处理） |
| Tydora | [zuorn/Tydora](https://github.com/zuorn/Tydora) | [01-single-file/tydora.md](01-single-file/tydora.md) | 01-single-file | v0.3.3（11-10），提交 11-10 | 协议 Apache-2.0；平台 / 数据真源 / AI 待补齐 |
| edgeever | [tianma-if/edgeever](https://github.com/tianma-if/edgeever) | [03-knowledge-base/edgeever.md](03-knowledge-base/edgeever.md) | 03-knowledge-base | v2.26.0（11-12），提交 11-14 | AGPL-3.0；自托管实例 + 内置 AI 已判定 |
| Trilium（TriliumNext） | [TriliumNext/Trilium](https://github.com/TriliumNext/Trilium) | [03-knowledge-base/triliumnext.md](03-knowledge-base/triliumnext.md) | 03-knowledge-base | v0.107.0（11-08），提交 11-14 | 主程序与 Web Clipper 各自发版，别混用版本号 |
| Blinko | [blinkospace/blinko](https://github.com/blinkospace/blinko) | [04-quick-notes/blinko.md](04-quick-notes/blinko.md) | 04-quick-notes | 1.8.9（11-05），提交 11-05（无变化） | [已确认] **未停更**（用户 2026-11-10 确认）；本周无新动静 |
| memos | [usememos/memos](https://github.com/usememos/memos) | [04-quick-notes/memos.md](04-quick-notes/memos.md) | 04-quick-notes | 26.11.0（11-01），提交 11-13（无新发版） | rc 转正，编辑器与配额体系变化待核实 |
| tolaria | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | [03-knowledge-base/tolaria.md](03-knowledge-base/tolaria.md) | 03-knowledge-base | alpha-v2026.11.13-alpha.0004（11-13），提交 11-14 | 仍为 Alpha、无版本号承诺；AGPL-3.0；vault + 远程后端（非裸 .md） |
| MarkText | [marktext/marktext](https://github.com/marktext/marktext) | [01-single-file/marktext.md](01-single-file/marktext.md) | 01-single-file | v0.24.0-rc.2（11-13，预发布）/ 稳定 v0.23.0，提交 11-14 | 10 月起从半停滞恢复密集发版 |
| Logseq | [logseq/logseq](https://github.com/logseq/logseq) | [03-knowledge-base/logseq.md](03-knowledge-base/logseq.md) | 03-knowledge-base | Nightly 20261025（10-25）/ 2.0.2（10-07），提交 11-14（无新发版） | Beta 仍 2.0.2；DB 版数据真源待持续观察 |
| solomd | [zhitongblog/solomd](https://github.com/zhitongblog/solomd) | [01-single-file/solomd.md](01-single-file/solomd.md) | 01-single-file | v5.0.21（11-12），提交 11-14 | 单人维护、近乎日更；MIT，内置 AI（MCP server + BYO-key） |
| NoteGen | [codexu/note-gen](https://github.com/codexu/note-gen) | [02-ai-editors/notegen.md](02-ai-editors/notegen.md) | 02-ai-editors | v0.39.2（11-01），提交 11-11（无新发版） | 桌面 beta / 移动端 alpha，入选门槛持续观察 |
| morrow | [StarrySky7D4/morrow](https://github.com/StarrySky7D4/morrow) | [01-single-file/morrow.md](01-single-file/morrow.md) | 01-single-file | 0.1.9-test.56（09-25，测试预览），提交 11-12（无发版） | 仅测试预览版，无正式 Release；AGPL-3.0；入选门槛待人类复核 |
| nomo | [nomo-md/nomo](https://github.com/nomo-md/nomo) | [01-single-file/nomo.md](01-single-file/nomo.md) | 01-single-file | v0.7.2（11-12），提交 11-13 | AGPL-3.0；数据真源本地 .md；平台待核 |

## 进展记录

| 日期 | 进展 | 来源 |
| --- | --- | --- |
| 2026-11-10 | 名单由旧定时任务融合进来，作为巡检第二真源建立；16 款中 8 款已收录、8 款记为候选 | 旧任务提示词与 `data/snapshot_2026-11-06.json` |
| 2026-11-10 | [已确认] 8 款候选全部转入正表（DEC-006），16 款均有主条目；Blinko 确认未停更；旧任务删除，调度改为每周六 09:00 | 用户 2026-11-10 指示 |
| 2026-11-14 | 首次真正联网核实（GitHub API / typoraio.cn）：Typora 无变化；10 款有更新（Obsidian / orca-note / Anytype / Tydora / edgeever / TriliumNext / tolaria / MarkText / solomd / nomo）；5 款无新发版（Blinko / memos / Logseq / NoteGen / morrow）；四字段补实 4 款（orca-note / Anytype / edgeever / tolaria） | GitHub API、typoraio.cn |
| 2026-11-14 | [已确认] 用户确认虎鲸笔记**闭源**、Anytype **按开源处理**，均保留正表（DEC-008）；协议字段同步更新 | 用户 2026-11-14 指示 |
