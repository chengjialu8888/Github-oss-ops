<div align="center">

# 🚀 github-oss-ops

**Your AI-Powered Open Source Growth Engine**

**你的 AI 开源项目增长引擎**

[![Platform](https://img.shields.io/badge/Platform-Mira%20%7C%20Claude%20Code%20%7C%20OpenClaw%20%7C%20Any%20Agent-blue)](#platform-setup)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](#license)
[![Skill Format](https://img.shields.io/badge/Format-SKILL.md%20(Universal)-orange)](#how-it-works)

Stop guessing. Start growing. A battle-tested playbook distilled into an AI skill that turns your GitHub project from invisible to unstoppable.

别再凭感觉运营了。一套经过实战验证的增长方法论，浓缩为 AI 技能，让你的 GitHub 项目从无人问津到势不可挡。

[English](#english) · [中文](#中文)

</div>

---

<a id="english"></a>

## Why This Skill Exists

Every day, thousands of open source projects are born on GitHub. Most die in obscurity — not because the code is bad, but because **nobody ever finds out about them**.

The gap between "great project" and "popular project" isn't code quality. It's **operations**: how you position, promote, and nurture your project into a self-sustaining community.

This skill bridges that gap. It encodes the collective wisdom from real-world open source growth playbooks into an AI assistant that sits inside your daily workflow — diagnosing your project's stage, generating tailored growth plans, writing your README, drafting your Hacker News launch post, and iterating with you as your metrics evolve.

### What Makes This Different

| Feature | Generic AI Advice | **github-oss-ops** |
|---------|-------------------|--------------------|
| Stage awareness | One-size-fits-all tips | Diagnoses your project phase (0→100 / 100→1K / 1K+) and adapts strategy |
| Actionable output | "Write better docs" | "Add an asciinema GIF to your README, publish to r/Python Tuesday 8am EST, expect +30 stars" |
| Anti-patterns | Might suggest star-gaming | 7 built-in guardrails against common traps (star-buying, spam posting, etc.) |
| Iteration loop | One-shot advice | Built-in PDCA cycle with checkpoints, failure diagnosis, and Plan B |
| Templates | "You should have a CONTRIBUTING.md" | Ships 6 production-ready templates (CONTRIBUTING, CoC, Issue/PR templates, SECURITY) |
| Multi-platform | Platform-locked | Runs on Mira, Claude Code, OpenClaw, or any SKILL.md-compatible agent |

### Core Capabilities

- **Project Diagnosis** — Automatically identifies your growth stage and bottlenecks
- **Growth Plan Generation** — 30-day quick wins + 90-day roadmap + metrics tracking table
- **README Rewriting** — Complete README.md with badges, benchmarks, quick start, and architecture diagrams
- **Content Operations** — Tech blogs, social media copy (Twitter/Reddit/HN), CFP proposals
- **Community Governance** — CONTRIBUTING.md, CODE_OF_CONDUCT, Issue/PR templates, SECURITY.md
- **Channel Strategy** — ROI-ranked promotion channels: HN, Reddit, Dev.to, Product Hunt, GitHub Trending
- **Trap Avoidance** — 7 anti-patterns actively flagged (star-gaming, spam, paid shilling, etc.)
- **Strategy Iteration** — PDCA loop with attribution analysis, failure modes, and channel tracking matrix

---

## How It Works

```
github-oss-ops/
├── SKILL.md                        # Core instructions (207 lines)
└── references/
    ├── growth-playbook.md          # Full strategy library (436 lines)
    └── templates.md                # Community governance templates (316 lines)
```

The skill follows the universal `SKILL.md` format — a YAML frontmatter for triggering metadata, followed by Markdown instructions that any LLM can follow. No proprietary APIs, no vendor lock-in, no code dependencies.

When triggered, the AI reads `SKILL.md` and follows a 4-step workflow:
1. **Diagnose** your project's current stage and bottlenecks
2. **Plan** a structured growth strategy with specific timelines and metrics
3. **Execute** by helping you write README, blogs, social posts, and governance docs
4. **Iterate** with built-in checkpoints and failure-mode analysis

---

## Platform Setup

### Mira (Bytedance)

**Already installed.** The skill is deployed at:
```
/opt/tiger/mira_nas/plugins/prod/{your_user_id}/skills/github-oss-ops/
```

**Trigger it** by saying things like:
- "我的开源项目怎么涨 Stars？"
- "帮我做个开源运营计划"
- "帮我优化 README"

Mira features: Full toolchain available — Feishu doc export, web browsing for repo analysis, web search for trend research, image generation for diagrams.

### Claude Code (Anthropic)

1. **Copy the skill folder** to your Claude Code custom skills directory:
   ```bash
   # Clone or copy the skill directory
   cp -r github-oss-ops/ ~/.claude/skills/github-oss-ops/
   ```

2. **Or use the `/skill` command** if your setup supports custom skill loading:
   ```
   /skill install github-oss-ops
   ```

3. **Trigger it** naturally in conversation:
   - "Help me grow my GitHub project's stars"
   - "Write a README for my Go framework"
   - "My open source project has stalled at 200 stars"

Claude Code features: File system access for saving plans as .md files, bash for running analysis scripts, web search via MCP.

### OpenClaw / Custom Agents

1. **Copy the skill directory** into your agent's skill path:
   ```bash
   cp -r github-oss-ops/ /path/to/your/agent/skills/
   ```

2. **Ensure your agent supports SKILL.md loading.** The skill uses standard YAML frontmatter + Markdown body format. If your agent reads `SKILL.md` files with `name` and `description` fields in the frontmatter, it will work out of the box.

3. **Reference file loading**: The skill references two files in `references/`. Your agent should be able to read these when the SKILL.md instructs it to. If not, you can inline the content into SKILL.md (though it will be longer).

### Any Other Agent / Manual Use

The skill is **pure Markdown** — no API calls, no compiled code, no runtime dependencies. You can use it with any LLM by:

1. Pasting the content of `SKILL.md` into your system prompt
2. Telling the LLM: "Follow these instructions to help me with open source project growth"
3. Providing the reference files when deeper guidance is needed

This works with ChatGPT, Gemini, local models, or any other LLM that can follow structured instructions.

---

## Example Interactions

**Early-stage project:**
> "I just published a Python CLI tool on GitHub, only 12 stars. How do I get to 100?"

→ Returns: Diagnosis (early stage), 4 quick-win actions with day-by-day timelines, 90-day roadmap, metrics tracking table, and "start today" priorities.

**README optimization:**
> "Optimize the README for my Go microservice framework — high performance, low memory"

→ Returns: Complete README.md with centered header, 6 badges, "Why this?" comparison table, feature list, Quick Start code, benchmarks, architecture diagram, and contributing guide.

**Growth plateau:**
> "My project has 500 stars but growth stalled. Only +10/month for the last 3 months."

→ Returns: Plateau diagnosis with 3 root causes, content sprint plan (4 articles in 2 weeks), contributor activation strategy, HN re-launch playbook, and 90-day roadmap to 1,000.

---

## License

MIT — use it, fork it, share it. If this skill helps your project grow, a star on the repo would be appreciated. 🙂

---

---

<a id="中文"></a>

## 为什么做这个 Skill

每天都有成千上万的开源项目在 GitHub 上诞生，但大多数都默默无闻地消亡了——不是因为代码不好，而是因为**根本没人发现它们**。

"好项目"和"火项目"之间的差距不是代码质量，而是**运营**：你如何定位、推广、培育你的项目，使它成为一个自循环的社区。

这个 Skill 就是来填补这个差距的。它将真实的开源增长实战经验浓缩为一个 AI 技能，嵌入到你的日常工作流中——诊断项目阶段、生成定制化增长计划、帮你写 README、起草 Hacker News 发布文案、并随着指标变化与你一起迭代。

### 核心差异

| 特性 | 通用 AI 建议 | **github-oss-ops** |
|------|-------------|---------------------|
| 阶段感知 | 千篇一律的建议 | 自动诊断项目阶段（0→100 / 100→1K / 1K+），匹配对应策略 |
| 可执行性 | "写好文档" | "用 asciinema 录终端 GIF 加到 README，周二早 8 点发 r/Python，预计 +30 stars" |
| 反模式防护 | 可能建议刷 star | 7 条内置护栏（禁止刷 star、垃圾推广、付费买量等） |
| 迭代机制 | 一次性建议 | 内置 PDCA 循环 + 检查点 + 失败归因 + Plan B |
| 模板库 | "你应该有个 CONTRIBUTING.md" | 附带 6 个可直接使用的标准模板 |
| 跨平台 | 平台锁定 | 支持 Mira、Claude Code、OpenClaw 及任何兼容 SKILL.md 的 Agent |

### 核心能力

- **项目诊断**——自动识别增长阶段和瓶颈
- **增长计划生成**——30 天速赢 + 90 天路线图 + 指标追踪表
- **README 重写**——完整的 README.md，含 Badge、Benchmark、Quick Start、架构图
- **内容运营**——技术博客、社交媒体文案（Twitter/Reddit/HN）、CFP 提案
- **社区治理**——CONTRIBUTING.md、CODE_OF_CONDUCT、Issue/PR 模板、SECURITY.md
- **渠道策略**——按 ROI 分层的推广渠道：HN、Reddit、Dev.to、Product Hunt、GitHub Trending
- **陷阱规避**——7 大反模式主动拦截
- **策略迭代**——PDCA 循环 + 归因分析 + 失败模式应对 + 渠道效果追踪

---

## 工作原理

```
github-oss-ops/
├── SKILL.md                        # 核心指令文件（207 行）
└── references/
    ├── growth-playbook.md          # 完整策略库（436 行）
    └── templates.md                # 社区治理模板库（316 行）
```

采用通用 `SKILL.md` 格式——YAML 前置元数据 + Markdown 指令正文。无私有 API 依赖，无厂商锁定，无代码依赖。

触发后，AI 按 4 步工作流执行：
1. **诊断**项目当前阶段和瓶颈
2. **规划**结构化增长策略，含具体时间线和量化指标
3. **执行**帮你写 README、博客、社交文案和治理文档
4. **迭代**通过内置检查点和失败模式分析持续优化

---

## 各平台配置指南

### Mira（字节跳动）

**已自动安装**，部署路径：
```
/opt/tiger/mira_nas/plugins/prod/{你的用户ID}/skills/github-oss-ops/
```

**触发方式**——直接对话：
- "我的开源项目怎么涨 Stars？"
- "帮我做个开源运营计划"
- "帮我优化 README"

Mira 特有能力：飞书文档导出、浏览器访问 GitHub 分析仓库、搜索引擎查趋势、图片生成。

### Claude Code（Anthropic）

1. **复制 Skill 文件夹**到 Claude Code 的自定义技能目录：
   ```bash
   cp -r github-oss-ops/ ~/.claude/skills/github-oss-ops/
   ```

2. **或使用 `/skill` 命令**（如果你的环境支持）：
   ```
   /skill install github-oss-ops
   ```

3. **触发方式**——自然对话：
   - "Help me grow my GitHub project's stars"
   - "Write a README for my Go framework"
   - "My project stalled at 200 stars"

Claude Code 特有能力：文件系统保存 .md 文件、Bash 脚本执行、MCP Web 搜索。

### OpenClaw / 自定义 Agent

1. **复制 Skill 目录**到你的 Agent 技能路径：
   ```bash
   cp -r github-oss-ops/ /path/to/your/agent/skills/
   ```

2. **确保 Agent 支持 SKILL.md 加载**。标准格式：YAML frontmatter + Markdown body，有 `name` 和 `description` 字段即可。

3. **参考文件加载**：Skill 引用了 `references/` 下的两个文件，Agent 需要能在指令引导下读取它们。如果不支持，可以将内容内联到 SKILL.md 中。

### 其他 Agent / 手动使用

本 Skill 是**纯 Markdown**——无 API 调用、无编译代码、无运行时依赖。任何 LLM 都能用：

1. 将 `SKILL.md` 内容粘贴到 System Prompt
2. 告诉 LLM："按照这些指令帮我做开源项目运营"
3. 需要深入指导时提供 references 文件内容

适用于 ChatGPT、Gemini、本地模型，或任何能遵循结构化指令的 LLM。

---

## 使用示例

**早期项目：**
> "我刚在 GitHub 上发布了一个 Python CLI 工具，目前只有 12 个 stars，怎么才能快速涨到 100？"

→ 输出：诊断（早期阶段）、4 条速赢行动含逐日时间线、90 天路线图、指标追踪表、"今天就开始"优先级。

**README 优化：**
> "帮我优化这个 Go 微服务框架的 README，主要特性是高性能和低内存占用"

→ 输出：完整 README.md，含居中标题、6 个 Badge、竞品对比表格、特性列表、Quick Start 代码、性能基准、架构图、贡献指南。

**增长停滞：**
> "我的项目有 500 stars 但增长停滞了，最近三个月每月只涨 10 个"

→ 输出：停滞诊断含 3 个根因分析、内容冲刺计划（2 周 4 篇文章）、贡献者激活策略、HN 重新发布 playbook、通往 1000 的 90 天路线图。

---

## License

MIT — 自由使用、Fork、分享。如果这个 Skill 帮到了你的项目，欢迎给个 Star 🙂
