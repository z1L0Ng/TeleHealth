# TeleHealth

**Conversational Health Acoustic Sensing｜对话健康声学感知**

研究自然对话中健康相关的声学表现：构建经人工核验的生成数据集，开发 detection 模型，并部署到手机、端侧和 Jetson 等设备。目标投稿 UbiComp/IMWUT，团队工作截止日期为 2027-02-01。

- Notion 项目页：https://app.notion.com/p/3ea309efda298128b817e75d9570ff49
- 项目起点：2026-10-16 与 Jingping 的会议记录 https://app.notion.com/p/3fc309efda2980f1b930f4d1fe172314
- 协作规则：[AGENTS.md](AGENTS.md)

## 当前状态

2026-10-22 清空工作区与 Notion，从 2026-10-16 的会议记录重新开始。之前的原型、调研和 Codex 任务记录都不再作为依据。

## 目录

| 路径 | 内容 |
| --- | --- |
| `AGENTS.md` | 所有 agent 共用的规则、角色与交接协议 |
| `CLAUDE.md` | 让 Claude Code 加载 `AGENTS.md` |
| `.gitignore` | 环境、模型、缓存、数据和音频不进 git |
| `docs/tasks/` | Claude 写给 Codex 的任务单与交接 |

新目录随任务创建，并在这里登记。
