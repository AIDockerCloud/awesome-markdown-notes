# OpenTodo

> 分类：[任务管理 / Todo（自托管）](README.md) · 主清单：[根 README.md](../../README.md)
> 最近核实：2026-11-10 · 信息来源：根 `README.md`「任务管理 / Todo（自托管）」 · 状态：收录

## 一句话定位

自托管任务管理应用，不是笔记编辑器。「你的任务、你的服务器」：一个小容器即可部署，数据集中在一个 `/data` 卷里的单个 SQLite 文件中，服务器负责同步、备份与共享，各设备离线时保留完整副本、联网后再同步。

## 四字段判定 [事实]

| 字段 | 内容 | 核实来源 |
| --- | --- | --- |
| 协议 | AGPL-3.0 | 主清单 |
| 平台 | 自托管服务器 + 各设备离线副本 | 主清单 |
| 数据真源 | **服务器** `/data` 卷里的单个 SQLite 文件；设备上是同步副本 | 主清单 |
| AI 形态 | —（未核实） | 主清单未给 |

## 要点 [事实]

- 项目：https://github.com/OpenTodoApp/OpenTodo
- 官方 Obsidian 插件 obsidian-opentodo（OpenTodoApp/obsidian-opentodo）的定位是把 Obsidian 当作**操作入口**：在 Obsidian 里看和改任务，但任务仍存 OpenTodo 服务器，不会变成 vault 里的笔记文件。
- 服务器负责同步、备份与共享；设备离线保留完整副本，联网后再同步。

## 归类理由与边界 [推断]

- 本节管的是任务本身，不是写笔记；收录它是因为常与笔记软件放在一起比较，而**任务到底存在哪里**完全不同，选错等于选错真源。
- 与 [TaskNotes](tasknotes.md)、[taskquence](taskquence.md) 的模型正好相反；与 [思源 Task Horizon](siyuan-task-horizon.md) 也不同（后者不另存任务数据）。
- 主清单提示：已经有一个任务真源时不要再开第二个；OpenTodo 与 TaskNotes 可经 vault 同步能力互相映射，但映射不等于双真源，以哪边为准要先定死。

## 待核实 [未决]

- AI 形态（四字段中唯一缺口）。
- 最近一次正式 Release 日期、近 6 个月提交活跃度。
- obsidian-opentodo 的映射方向是否仍为单向真源。

## 进展记录

| 日期 | 进展 | 来源 |
| --- | --- | --- |
| 2026-11-10 | 初版收录，信息核实自主清单 | 根 `README.md` |
