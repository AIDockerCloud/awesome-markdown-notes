# 工程智能体规范 (AGENTS.md — PCMP Lite)

## 项目定位

`awesome-markdown-notes` 是一份按用途分层的 Markdown 编辑器与笔记软件精选清单，**唯一对外产物是根目录 `README.md`**。
本项目采用 **PCMP Lite**（极简 4 件套）：纯 Markdown 驱动、零构建、零依赖、零运行时。

## 关键路径

- 生效协议原版：[PROJECT_CONTEXT_ZH.md](PROJECT_CONTEXT_ZH.md) / [PROJECT_CONTEXT.md](PROJECT_CONTEXT.md)（模板，勿改）
- 项目硬约束：[ai/PROJECT.md](ai/PROJECT.md)
- 状态与活动任务：[ai/STATE.md](ai/STATE.md)（接管必读，Lite 档位已合并 TASK）
- 决策真源：[ai/DECISIONS.md](ai/DECISIONS.md)
- 清单正文：[README.md](README.md)

## 工程硬事实

- 无构建、无测试、无依赖、无 CI 脚本；仓库里没有 `package.json` 与 `node_modules/`。
- 内容变更只落 `README.md`；上下文变更只落 `ai/` 与 `AGENTS.md`。
- Git 远端：`https://github.com/AIDockerCloud/awesome-markdown-notes.git`。
- 所有 `ai/` 路径相对项目根目录解析；动态文件带 `pcmp_version` / `revision` / `updated` Frontmatter。
- 协议版本：PCMP v2.2（2026-10-20）。

## 智能体协作守则

1. **接管必读顺序**：`PROJECT_CONTEXT_ZH.md` ➔ `ai/PROJECT.md`（硬约束） ➔ `ai/STATE.md`（状态 + 当前任务） ➔ `ai/DECISIONS.md` 中相关 Accepted 决策。严禁只读状态摘要就推测系统约束。
2. **状态合一**：Lite 档位不建 `TASK.md`，任务目标、验收勾选与 Next Action 直接写在 `ai/STATE.md`。
3. **信息分层**：显式使用 `[事实]` / `[假设]` / `[提议]` / `[已确认]` / `[未决]`；AI 建议未经人类确认不得记为 `[已确认]` 或 Accepted ADR。
4. **决策留痕**：收录口径、分区结构、命名与 Topics 等口径变更必须在 `ai/DECISIONS.md` 登记 ADR，并附确认来源。
5. **收尾更新**：任务完成后递增 `ai/STATE.md` 的 `revision`，更新完成项与即时下一步；本档位不建 `sessions/`，审计靠 Git 提交说明。
6. **中文写作**：自然、简短、准确，只写可判定的结构性事实；任务回执分「做完了 / 需要你 / 知会」三段，结论先行。

## 红线与禁区

1. **协议原版保护**：严禁修改根目录 `PROJECT_CONTEXT*.md`；需定制时复制完整副本到 `ai/` 作为项目使用版。
2. **不得弱化免责声明**：README 开头「与 Typora 无关联、未获其背书或赞助」及商标说明不得删除，也不得改写为暗示官方关联。
3. **不擅自扩表**：新增条目须先过 `ai/PROJECT.md` 的入选门槛与四字段可判定检查，判定不了的只记候选，不进正表。**例外须人类明确指示**：2026-11-10 用户确认把 8 款候选批量转入正表（DEC-006）、TypeOpen 四字段未齐仍保留正表（DEC-007），四字段一律显式写 `—（未核实）`；闭源无公开仓库的产品按官网发布记录判定活跃度（DEC-007）。详见 `ai/DECISIONS.md`。
4. **不写易过期信息**：正文只写结构性事实（协议、平台、数据真源、AI 形态），价格与具体版本不进正文。
5. **审阅授权**：审阅、审计或验活的对象由人类指定；未获许可不得擅自扩大范围或改动未点名的条目。

## 常用命令

- 变更核对：`git status --short && git diff -- README.md`
- 接管提示词：`请按 PCMP Lite 接管本项目：阅读 PROJECT_CONTEXT_ZH.md、ai/PROJECT.md、ai/STATE.md，列出未决问题后继续推进当前任务。`
- 未引入派生工具：Lite 档位不启用 `scripts/pcmp_index.py`，合规靠人工核对 Frontmatter 与 ADR 字段。

## 分类目录与产品卡片（内容层）

- 内容真源分两层：**主清单** `README.md`（按用途分层，每条只记四字段）与 **`categories/`**（每款软件一张卡片 + 每类一张对比清单）。
- 目录编号：`00-baseline`、`01-single-file`、`02-ai-editors`、`03-knowledge-base`、`04-quick-notes`、`05-task-management`、`06-references`。
- `categories/<NN>-<slug>/README.md` 是该类**对比清单**，也是每周核实的对象清单；`<软件>.md` 是产品卡片。
- `categories/_TEMPLATE.md` 是卡片模板，新增软件照它复制，不要手写新格式。
- `categories/06-references/` 是外部索引资源（清单 / 目录站 / 测评文），不是软件，不建产品卡片。
- `CHANGELOG.md` 是每周进展汇总的唯一写入点。

### 新增软件流程（人类不定时增加时用）

1. 判断归属分类；跨界的只在一处写完整介绍，其它分区一句话指回主条目。
2. 复制 `categories/_TEMPLATE.md` 到该分类目录，文件名用小写连字符（如 `obsidian.md`）。
3. 四字段判定不了写 `—（未核实）`，**不要猜**；有关键缺失时状态记「候选」，是否进主清单正表由人类确认（2026-11-10 有一次人类确认的批量转正，见 DEC-006）。
4. 在该分类 `README.md` 对比表补一行并链接到卡片；任务管理类还要补「任务真源对照」表。
5. 根 `README.md` 是否新增条目由人类确认；分类清单与卡片可以先建。
6. 只写结构性事实，不写价格、具体版本号、发布日期；链接优先指向项目主页 / 仓库根地址。
7. 收尾时递增 `ai/STATE.md` 的 `revision`。

### 巡检观察名单（内容层）

- `categories/_WATCHLIST.md` 是**巡检对象第二真源**：2026-11-10 由旧定时任务「笔记软件更新进展」融合进来，登记 16 款软件及上游地址。
- [已确认] 16 款已于 2026-11-10 全部经人类确认转入正表（DEC-006）：新建 8 张产品卡片、补入分类对比表与主清单；四字段未判定者一律 `—（未核实）`。
- [事实] 后续新增「候选」状态的对象只记录进展，是否升级由人类确认；名单落在仓库文件里，不写死在定时任务提示词中。

### 每周进展更新约定

- 定时任务**每周六 09:00** 运行（ID `b7a78148…`；2026-11-10 与旧「笔记软件更新进展」任务融合，旧任务已删除）。检查对象有**两处真源**：`categories/*/README.md` 对比表（**动态发现**，不写死名单）与 `categories/_WATCHLIST.md`（16 款含上游地址）。
- 每轮先读 `CHANGELOG.md` 最新一节、各分类「进展」表最后一行与 `_WATCHLIST.md` 的「上次快照」列作为基线，逐款给出「有更新 / 无变化 / 未核实到」，**写清更新了什么**，不只写版本号。
- 写入点：根 `CHANGELOG.md` 汇总（含状态对照表）、各分类 `README.md` 的「进展」表、有实质变化的产品卡片「进展记录」表、`_WATCHLIST.md` 的「上次快照」列。
- 硬约束：只写可核实且带来源的事实，核实不到写「未核实到」；发现停更 / 归档 / 协议变化只标注并提请人类确认，**不自动删除或移出条目**；候选对象不自动升级；Blinko 已于 2026-11-10 经人类确认「未停更」，不再把历史停更判断当作待确认项；不改协议原版，不改主清单现有条目。
- 成本：GitHub `releases.atom` / `commits.atom` 轻量 feed 优先，Typora / Obsidian 用官方发布页与 changelog；不 clone、不下载二进制；本机蜂窝热点有流量配额，核实不到不反复重试。
- 历史产出回填须标注「历史回填（未联网复核）」与原始文件名，不得当作本轮核实结论。
- 改动留在工作区供人类 review，定时任务不执行 `git commit`。
