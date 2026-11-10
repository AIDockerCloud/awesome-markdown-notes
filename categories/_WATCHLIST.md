# 巡检观察名单 (_WATCHLIST)

> 最近更新：2026-11-10 · 状态：[已确认] 16 款全部经人类确认转入正表
> 用途：**每周巡检对象的第二真源**，与 `categories/*/README.md` 的对比表并列。定时任务同时遍历两处，不依赖写死在任务提示词里的名单。
> 来源：旧任务「笔记软件更新进展」（每周五 18:00，2026-10-07 起运行 5 次），2026-11-10 融合进项目任务（每周六 09:00）后已删除。

## 使用口径

- [事实] 表内每一行都是本周要核实的对象，核实结论写入根 `CHANGELOG.md`，并更新本文件「上次快照」列。
- [已确认] 2026-11-10 原 8 款候选全部经人类确认转入正表，已建产品卡片、补入分类对比表与主清单；四字段未判定者一律写 `—（未核实）`，不猜测填充（DEC-006）。
- [事实] 后续若有新对象，可先记为「候选」只记录进展；是否升级为收录由人类确认，规则见 [AGENTS.md](../AGENTS.md)。
- [事实] 「上次快照」是 2026-11-06 的历史回填基线，来源 `data/snapshot_2026-11-06.json`，**本轮未做新的联网核实**；每周任务核实后覆盖此列。
- [事实] 本文件只登记对象与基线，不写价格、不写主观评价；详细进展与来源写在 `CHANGELOG.md` 与产品卡片。
- [事实] `06-references` 的外部索引资源不在此表内，仍按分类清单单独核实链接可达性与口径变化。

## 巡检对象（16 款，均已收录）

| 软件 | 上游地址 | 主条目 | 分类 | 上次快照（2026-11-06） | 备注 |
| --- | --- | --- | --- | --- | --- |
| Typora | [官方发布页](https://typora.io/releases/stable.html) | [00-baseline/typora.md](00-baseline/typora.md) | 00-baseline | 1.14.15 稳定 / 1.14.4-dev（11-06） | 闭源，无公开仓库；[已确认] 活跃度按官网发布记录判定（DEC-007）；`typora.io` DNS 异常时走官方中文站同页 |
| Obsidian | [obsidianmd/obsidian-releases](https://github.com/obsidianmd/obsidian-releases) | [03-knowledge-base/obsidian.md](03-knowledge-base/obsidian.md) | 03-knowledge-base | 1.15.0（11-02） | 闭源，用发布镜像仓库与官方 changelog 核实 |
| 虎鲸笔记 orca-note | [sethyuan/orca-note](https://github.com/sethyuan/orca-note) | [03-knowledge-base/orca-note.md](03-knowledge-base/orca-note.md) | 03-knowledge-base | 1.100.0（11-05），公开仓库提交停 2026-07-10 | 只发 Release 不推源码，GitHub 活跃度无参考价值；四字段待核实 |
| Anytype | [anyproto/anytype-ts](https://github.com/anyproto/anytype-ts) | [03-knowledge-base/anytype.md](03-knowledge-base/anytype.md) | 03-knowledge-base | v0.57.7（11-03），提交 11-03 | 数据真源是否为裸 `.md` 待核实 |
| Tydora | [zuorn/Tydora](https://github.com/zuorn/Tydora) | [01-single-file/tydora.md](01-single-file/tydora.md) | 01-single-file | v0.3.2（10-12），提交 10-12 | 低频维护，入选门槛待复核 |
| edgeever | [tianma-if/edgeever](https://github.com/tianma-if/edgeever) | [03-knowledge-base/edgeever.md](03-knowledge-base/edgeever.md) | 03-knowledge-base | v2.21.0（11-05），提交 11-06 | 1.x → 2.0 为破坏性变更；自托管真源与 AI 架构待核实 |
| Trilium（TriliumNext） | [TriliumNext/Trilium](https://github.com/TriliumNext/Trilium) | [03-knowledge-base/triliumnext.md](03-knowledge-base/triliumnext.md) | 03-knowledge-base | v0.106.1（10-23），提交 11-05 | 主程序与 Web Clipper 各自发版，别混用版本号 |
| Blinko | [blinkospace/blinko](https://github.com/blinkospace/blinko) | [04-quick-notes/blinko.md](04-quick-notes/blinko.md) | 04-quick-notes | 1.8.9（11-05），提交 11-05 | [已确认] **未停更**（用户 2026-11-10 确认），历史停更判断不成立 |
| memos | [usememos/memos](https://github.com/usememos/memos) | [04-quick-notes/memos.md](04-quick-notes/memos.md) | 04-quick-notes | 26.11.0（11-01），提交 11-06 | rc 转正，编辑器与配额体系变化待核实 |
| tolaria | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | [03-knowledge-base/tolaria.md](03-knowledge-base/tolaria.md) | 03-knowledge-base | Alpha 2026.11.6.2（11-06），提交 11-06 | 仍为 Alpha、无版本号承诺；vault 存储格式待核实 |
| MarkText | [marktext/marktext](https://github.com/marktext/marktext) | [01-single-file/marktext.md](01-single-file/marktext.md) | 01-single-file | v0.24.0-rc.1（11-03），提交 11-06 | 10 月起从半停滞恢复密集发版 |
| Logseq | [logseq/logseq](https://github.com/logseq/logseq) | [03-knowledge-base/logseq.md](03-knowledge-base/logseq.md) | 03-knowledge-base | Nightly 20261025，提交 11-06 | Beta 仍 2.0.2；DB 版数据真源待持续观察 |
| solomd | [zhitongblog/solomd](https://github.com/zhitongblog/solomd) | [01-single-file/solomd.md](01-single-file/solomd.md) | 01-single-file | v5.0.13（11-03），提交 11-04 | 单人维护、近乎日更；四字段待核实 |
| NoteGen | [codexu/note-gen](https://github.com/codexu/note-gen) | [02-ai-editors/notegen.md](02-ai-editors/notegen.md) | 02-ai-editors | v0.39.2（11-01），提交 11-04 | 桌面 beta / 移动端 alpha，入选门槛持续观察 |
| morrow | [StarrySky7D4/morrow](https://github.com/StarrySky7D4/morrow) | [01-single-file/morrow.md](01-single-file/morrow.md) | 01-single-file | 0.1.9-test.56（09-25），提交 10-05 | 仅测试预览版，无正式 Release；入选门槛待复核 |
| nomo | [nomo-md/nomo](https://github.com/nomo-md/nomo) | [01-single-file/nomo.md](01-single-file/nomo.md) | 01-single-file | v0.6.2（10-16），提交 10-23 | 四字段待核实 |

## 进展记录

| 日期 | 进展 | 来源 |
| --- | --- | --- |
| 2026-11-10 | 名单由旧定时任务融合进来，作为巡检第二真源建立；16 款中 8 款已收录、8 款记为候选 | 旧任务提示词与 `data/snapshot_2026-11-06.json` |
| 2026-11-10 | [已确认] 8 款候选全部转入正表（DEC-006），16 款均有主条目；Blinko 确认未停更；旧任务删除，调度改为每周六 09:00 | 用户 2026-11-10 指示 |
