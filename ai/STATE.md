---
pcmp_version: "2.2"
revision: 8
updated: 2026-11-14
---

# 项目当前状态与活动任务快照 (STATE.md — Lite)

- **Last Updated**: 2026-11-14
- **Overall Status**: 2026-11-14 完成**首轮真正联网核实**（GitHub API / typoraio.cn）：遍历 32 款对比表对象 + 16 款观察名单，相对 2026-11-06 基线逐款对比，得出 10 款有更新、5 款无新发版（Blinko / memos / Logseq / NoteGen / morrow）、4 款四字段补实（orca-note / Anytype / edgeever / tolaria）；Typora 稳定版无变化。DEC-001 ~ 009 均 Accepted，无 Proposed；DEC-008（虎鲸闭源 / Anytype 开源）、DEC-009（morrow / tolaria 保留正表）已定案。**本轮改动按人类指示提交并推送远程**。

---

## 当前唯一活动任务 (Active Task)

> Lite 档位特性：活动任务合并维护在此，不建独立 `TASK.md`。

- **任务名称**：2026-11-14 每周产品进展核实（首轮真正联网）
- **背景与范围**：按定时任务遍历 `categories/*/README.md` 对比表（32 款）与 `_WATCHLIST.md`（16 款），以 2026-11-06 快照为基线逐款对比（有更新 / 无变化 / 未核实到）；重点补齐 8 款转正软件的四字段。仅做轻量 HTTP 核实，不 clone、不下载二进制。
- **约束与非目标**：不改主清单 `README.md` 现有条目、不改协议原版、不执行 `git commit`；只写可核实且带来源的事实，核实不到写「未核实到」。
- **关联文件**：`CHANGELOG.md`、`categories/*/README.md`、`categories/*/<slug>.md`、`categories/_WATCHLIST.md`、`ai/STATE.md`
- **验收标准**：
  - [x] `CHANGELOG.md` 追加 2026-11-14 小节，含全部检查对象状态对照表 + 更新「上次快照」基线；
  - [x] 各分类 `README.md`「进展」表追加本周行；
  - [x] 11 张有实质变化的产品卡片更新四字段 + 进展记录（Aropyt / TypeOpen / MarkFlowy / Tydora / solomd / morrow / nomo / orca-note / Anytype / edgeever / tolaria）；
  - [x] `_WATCHLIST.md`「上次快照」列更新为 2026-11-14；
  - [x] `ai/STATE.md` 的 `revision` 递增至 6。

---

## 已完成里程碑 (Completed)

- [已确认] 2026-11-10 提交 `788a05c`：发布 `README.md` 初版，含 8 个分区与「收录标准与维护方式」。
- [已确认] 2026-11-10 完成 PCMP Lite 初始化；档位选择登记为 DEC-002（现 Accepted）。
- [已确认] 2026-11-10 完成分类目录 / 产品卡片 / 对比清单 / CHANGELOG / 每周定时任务；结构与机制登记为 DEC-003、DEC-004（现均 Accepted）。
- [已确认] 2026-11-10 完成两个定时任务融合与历史进展回填，DEC-005 转 Accepted。
- [已确认] 2026-11-10 完成融合收尾的四项变更，登记为 DEC-006（Accepted）。
- [已确认] 2026-11-10 人类逐项确认待确认项：DEC-002 / 003 / 004 转 Accepted，新增 DEC-007；TypeOpen 保留正表、Typora 门槛按官网判定。
- [已确认] 2026-11-14 完成首轮真正联网核实：32 款全部核实，10 款有更新、5 款无新发版；8 款转正软件 + Aropyt / TypeOpen / MarkFlowy 四字段补实（个别平台项仍待核）；CHANGELOG / 各分类进展表 / `_WATCHLIST` 上次快照 / 11 张卡片全部更新。
- [已确认] 2026-11-14 用户确认：虎鲸笔记**闭源**、Anytype **按开源处理**，均保留正表（DEC-008）；协议字段已同步卡片、分类表、`_WATCHLIST`、`CHANGELOG`。
- [已确认] 2026-11-14 用户确认 morrow / tolaria **保留正表**（DEC-009），入选门槛例外维持；本轮无剩余待确认项。

## 进行中 (In Progress)

- 无。等待人类 review 与提交。

## 阻塞项 (Blocked)

- 无。DEC-001 ~ 007 均为 Accepted，无 Proposed 决策，也无技术阻塞。

## 当前风险与焦点 (Current Risks & Focus)

- [事实] **四字段缺口已大幅收窄**：8 款转正软件 + Aropyt / TypeOpen / MarkFlowy 已补实；01-single-file 齐全度 8/9、03-knowledge-base 11/12。剩余待核：Tydora（平台 / 数据真源 / AI）、nomo（平台）、Anytype（平台 / AI）、tolaria（AI）、ghostwriter（AI）、虎鲸笔记（平台 / 数据真源）。
- [已确认] **入选门槛例外已定案**：morrow（仅测试预览版）、tolaria（仅 Alpha）均按人类确认保留正表（DEC-009），不转候选、不自动移出；虎鲸笔记已确认闭源（DEC-008），按 DEC-007 以 Release 判定、视为活跃；Anytype 按开源处理（DEC-008）。
- [事实] **本轮已真正联网核实**（GitHub API / typoraio.cn）；但 GitHub 未鉴权 API 60 次/小时，后半段（Aropyt / TypeOpen / Nimbalyst / MarkFlowy / 思源 Task Horizon / TaskNotes 精确发版）触发 403，相关版本号改用官网 / 商店页 / 镜像站二手源交叉核实并已标注。
- [事实] **两处巡检真源已同步**：本轮同时更新 `categories/*/README.md` 对比表与 `_WATCHLIST.md` 上次快照列，未发现分叉。
- [事实] **代理约束**：本机代理放行 `api.github.com` / `raw.githubusercontent.com`，但拦截 `github.com` 主站与 `typora.io`；06-references 中 alternativeto.net / producthunt.com 返回 403（疑似反爬，非明确失效），下周可换 UA 或直连复查。
- [已确认] Blinko **未停更**（11-05 发 1.8.9）；本周无新发版，仍属正常区间。
- [已确认] TypeOpen **保留正表**、Typora 等闭源产品**按官网发布记录判定活跃度**（DEC-007）；本周 Typora 经 typoraio.cn 判定为 1.14.15、无变化。
- [事实] 定时任务每周六 09:00 运行；提示词沿用轻量 HTTP / API、不 clone、不下载二进制、不反复重试，蜂窝热点流量配额仍是硬约束。
- [事实] 主清单至少 9 条链接锚定到易变目标，「链接去版本化」尚未实施。
- [事实] `git status` 显示本轮改动均在工作区未提交；`.workbuddy/` 仍为未跟踪目录，提交前建议决定是否加入 `.gitignore`。

## 下一步即时动作 (Immediate Next Action)

- [未决] 人类 review 本轮产物并提交（本轮与定时任务均不自动 `git commit`）；提交前先决定是否把 `.workbuddy/` 加入 `.gitignore`。
- [未决] **下周六 09:00** 以上一轮 2026-11-14 快照为锚点继续逐款核实；优先补齐 Tydora / nomo / Anytype / tolaria / ghostwriter / 虎鲸笔记 剩余字段，并复查 alternativeto / producthunt 链接。
- [已确认] morrow / tolaria 保留正表（DEC-009）；虎鲸笔记闭源、Anytype 开源（DEC-008），均无剩余待确认项。下一步仅需例行每周巡检。
- [未决] 若核实发现归类不符或某款确实停更 / 归档，只标注并提请人类确认，不自动移出条目。
