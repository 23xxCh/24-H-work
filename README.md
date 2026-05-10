# 24-H-work

24小时自动化开发迭代 SKILL，让 AI 不知疲倦地为你的想法工作。

## 核心特性

- **24小时持续运行** — 无人值守，自动迭代
- **竞品超越** — 深度分析所有竞品，目标是全面超越
- **13阶段标准流程** — CEO Plan → Adversarial Review → Eng Plan → Design → Implement → Ship → QA → Score
- **对抗性审查** — 双重 AI 挑战，找出潜在问题
- **多轮迭代** — 每轮分数持续上升
- **6维度评分** — 功能、代码质量、测试覆盖、UX、需求符合、设计质量
- **断点续连** — 重启后可从断点继续

## 融合的最佳实践

本 SKILL 融合了以下开源项目的核心设计理念：

- [Ralph](https://github.com/snarktank/ralph) (18.2k stars) — PRD 驱动的自主开发循环
- [gstack-auto](https://github.com/loperanger7/gstack-auto) (188 stars) — 13阶段流程 + 对抗性审查
- [Continuous Agent Loop](https://github.com/affaan-m/everything-claude-code) — 质量门禁 + 评估循环
- [Continuous Learning](https://github.com/AlexMikhalev/claude-code-continuous-learning-skill) — 自我改进和知识提取

## 开始使用

### 1. 克隆到本地

```bash
git clone https://github.com/23xxCh/24-H-work.git ~/.claude/skills/24-floating-shamir
```

### 2. 在 Claude Code 中启动

```
/24-floating-shamir
```

### 3. 描述你的想法

告诉 SKILL 你想做什么，它会自动：

1. 调研市场竞品
2. 生成需求文档（PRD）
3. 分解任务清单
4. 执行 13 阶段开发流程
5. 持续迭代直到超越所有竞品

## 工作流程

```
Phase 0: 竞品调研（必须首先执行）
    ↓
Phase 1: 初始化 → PRD.md + tasks.md
    ↓
Phase 2: 多轮迭代开发（13阶段）
    ├── CEO Plan
    ├── Adversarial Review
    ├── Engineering Plan
    ├── Adversarial Review
    ├── Design Plan
    ├── Adversarial Review
    ├── Engineering Plan v2
    ├── Adversarial Review
    ├── Implement
    ├── Ship
    ├── QA (Bug 修复循环)
    ├── Document
    └── Score
    ↓
Phase 3: 轮次间迭代（分数持续上升）
    ↓
停止条件: 竞品超越完成 / 用户停止 / 分数达标
```

## 项目文件

```
24-H-work/
├── CLAUDE.md                    # Agent skills 配置
├── README.md                    # 本文件
├── skills/
│   └── 24-floating-shamir/
│       └── skill.md             # 核心 SKILL 文件
└── docs/
    └── agents/                  # 工程技能配置
        ├── issue-tracker.md
        ├── triage-labels.md
        └── domain.md
```

## 质量门禁

每轮产出必须通过：

- [ ] 代码可运行（无语法错误）
- [ ] 基本测试覆盖
- [ ] 无明显 bug
- [ ] 通过 lint/style 检查
- [ ] 符合 PRD 验收标准

## 评分系统

6 维度评分（每维度 1-10）：

| 维度 | 说明 |
|------|------|
| Functionality | 功能完整性 |
| Code Quality | 代码质量 |
| Test Coverage | 测试覆盖 |
| UX Polish | 用户体验 |
| Spec Adherence | 需求符合度 |
| Design Quality | 设计质量 |

**总分**: 60/60 = 超越所有竞品

## 定期汇报

SKILL 每完成一个阶段或每 15 分钟向用户报告进度。

## 停止条件

- 所有任务完成
- 所有竞品的优点已实现，且至少一维领先
- 连续两轮分数没有提升
- 用户主动停止

---

*让 AI 为你工作 24 小时，醒来时收获超越所有竞品的产品。*