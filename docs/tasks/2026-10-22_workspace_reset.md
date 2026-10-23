# 交接：工作区和 Notion 已清空，项目从头开始

- 日期：2026-10-22
- 发出：Claude 管理线程（由用户转达）
- 接收：所有 TeleHealth 的 Codex 线程，包括原管理线程 `01a0ef8b-741b-7632-914b-dbdfcefff5cc`、文献与数据调研、任务与评价设计、TTS、AMI局部增强声学分析、本科生对接

## 发生了什么

1. **本地仓库已清空。** 原来的 `analysis/`、`codex/`（包括 `thread_registry.json`）、`docs/` 和 `tts/` 都已移出仓库。`.git` 历史和 remote 保留。
2. **仓库从四个文件重新开始：** `.gitignore`、`README.md`、`AGENTS.md`、`CLAUDE.md`，以及本交接文件。
3. **Notion 已重建。**
   - 项目页更名为 “Conversational Health Acoustic Sensing｜对话健康声学感知”，URL 不变：https://app.notion.com/p/3ea309efda298128b817e75d9570ff49
   - 页面只有 Meeting Record、Working Plan、Meeting Report 三个板块；原来的数据库和子页面都已移入 Notion 回收站。
   - 三个板块中只保留 “2026-10-16 Jingping Meeting Record”（URL 不变），作为项目起点。

## 对 Codex 的影响

- `thread_registry.json` 里的所有任务、授权、范围和等待游标全部作废。之前的原型（Dia 生成、AMI 局部增强、SV 分析、数据集调研、GPT6Pro 调研包）不再作为依据。不要恢复或引用这些旧材料。
- 管理职责移交给 Claude 管理线程，包括与用户沟通、维护 Notion 和编写任务单。原 Codex 管理线程不再承担管理工作。Codex 线程不写 Notion，也不再维护线程登记。
- Codex 只作为执行线程：按 `docs/tasks/` 下的任务单工作，并在输出目录中写 `DELIVERY.md`。具体规则见 `AGENTS.md`。
- **现在没有分配给 Codex 的任务。** 在收到新的任务单之前，不建环境、不下载、不跑推理或训练，也不改动仓库。
- 本科生对接线程原有的上下文基于旧材料，如果要继续，也等待新的任务单。

## 新的起点

2026-10-16 与 Jingping 的会议记录：

- 三个可能的 contribution：人工核验的生成数据集；detection；部署（手机、端侧、Jetson 等）。
- Roadmap：考虑 4 种不同的生成方法 → 合成小规模数据集 → 交给 Wade 等人试听 → 约 20 人 user study → IRB → UbiComp 完整论文（目标约 20 个 figure+table）→ detection model → 部署到各种设备。
- DDL：2027-02-01。

具体方法、数据、模型和设备都还没有确定。

## 需要 Codex 做的

1. 阅读 `AGENTS.md` 和本文件。
2. 回复用户一句确认：已知晓重置、旧任务全部结束、正在等待新任务单。除此之外不做其他事。
