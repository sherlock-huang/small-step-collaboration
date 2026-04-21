# small-step-collaboration

让 Agent 在和用户协作时，一次只推进一个最小动作，而不是一次性甩出一大段 SOP。  
Make an agent guide a human one small step at a time instead of dumping a long SOP.

由 **鲲鹏AI探索局 / Kunpeng AI Lab** 创建并维护。  
Created and maintained by **鲲鹏AI探索局 / Kunpeng AI Lab**.

---

## 中文说明

### 这是什么

`small-step-collaboration` 是一份跨运行时的 skill bundle，目标不是给 Agent 增加一个新工具，而是让 Agent 换一种和用户配合的方式。

它优先适配：

- Codex
- OpenClaw
- Hermes

### 它解决什么问题

很多 Agent 的问题不是不会做事，而是不会带着用户一起做事。

常见问题包括：

- 一次性输出太多步骤
- 同时给很多分支方案
- 一口气要用户提供多种截图、日志、命令结果
- 在高风险操作前没有先做安全确认

这份 skill 会把默认交互方式改成：

1. 一次只给一个最小可执行动作
2. 一次只要一个结果
3. 解释当前结果意味着什么
4. 再给下一步

### 适合哪些场景

- Google Search Console
- Bing Webmaster Tools
- 百度搜索资源平台
- Cloudflare / Vercel / GitHub / 数据库后台
- 安装配置、部署发布、后台排障、索引验证

### 仓库内容

- `SKILL.md`：核心触发描述与行为规则
- `agents/openai.yaml`：Codex 的 UI 元数据
- `references/platform-notes.md`：平台安装说明
- `references/response-patterns.md`：可复用回复模板
- `_meta.json`：轻量发布元数据
- `docs/RELEASE_PACK.md`：对外发布技术说明

### 安装方式

#### Codex

把本文件夹复制到：

```text
~/.codex/skills/small-step-collaboration
```

#### OpenClaw

把本文件夹复制到：

```text
~/.openclaw/skills/small-step-collaboration
```

#### Hermes

把本文件夹复制到：

```text
~/.hermes/skills/small-step-collaboration
```

### 调用示例

```text
用 small-step collaboration 模式带我操作，一次只给我下一步。
```

或者：

```text
Use $small-step-collaboration and take me through this console one step at a time.
```

### 相关链接

- 主站技能页：https://kunpeng-ai.com/skills/small-step-collaboration/
- 下载包：https://kunpeng-ai.com/downloads/small-step-collaboration-skill.zip
- 技术说明文章：https://kunpeng-ai.com/blog/small-step-collaboration-skill-guide/
- 传播文章：https://kunpeng-ai.com/blog/why-agents-should-guide-users-one-step-at-a-time/
- 鲲鹏AI探索局主页：https://kunpeng-ai.com/
- Kunpeng Agent Forum：https://forum.kunpeng-ai.com/

### 署名

- 发布者：鲲鹏AI探索局 / Kunpeng AI Lab
- 网站：https://kunpeng-ai.com/
- 论坛：https://forum.kunpeng-ai.com/
- GitHub Owner：https://github.com/sherlock-huang

---

## English

### What This Is

`small-step-collaboration` is a cross-runtime skill bundle. It does not add a new tool capability by itself. Instead, it changes how an agent collaborates with a human user.

It currently targets:

- Codex
- OpenClaw
- Hermes

### What Problem It Solves

Many agents are capable, but not collaborative enough.

Typical failure modes include:

- dumping too many steps at once
- presenting multiple branches too early
- asking for too many screenshots, logs, and outputs in one turn
- skipping a safety checkpoint before risky actions

This skill shifts the default interaction style to:

1. give one smallest useful next action
2. ask for one result artifact
3. explain what the result means
4. continue with the next step

### Best-Fit Scenarios

- Google Search Console
- Bing Webmaster Tools
- Baidu Search Resource Platform
- Cloudflare / Vercel / GitHub / database consoles
- setup, deployment, debugging, and indexing verification

### Repository Contents

- `SKILL.md` - core trigger description and behavior rules
- `agents/openai.yaml` - Codex UI metadata
- `references/platform-notes.md` - runtime install notes
- `references/response-patterns.md` - reusable response patterns
- `_meta.json` - lightweight release metadata
- `docs/RELEASE_PACK.md` - technical release sheet

### Install

#### Codex

Copy this folder into:

```text
~/.codex/skills/small-step-collaboration
```

#### OpenClaw

Copy this folder into:

```text
~/.openclaw/skills/small-step-collaboration
```

#### Hermes

Copy this folder into:

```text
~/.hermes/skills/small-step-collaboration
```

### Example Invocation

```text
Use small-step collaboration mode for this task. Give me only the next smallest useful step, wait for my result, then guide the next step.
```

Or:

```text
Use $small-step-collaboration and take me through this console one step at a time.
```

### Public Links

- Skill landing page: https://kunpeng-ai.com/skills/small-step-collaboration/
- Download bundle: https://kunpeng-ai.com/downloads/small-step-collaboration-skill.zip
- Technical guide: https://kunpeng-ai.com/blog/small-step-collaboration-skill-guide/
- Why this matters: https://kunpeng-ai.com/blog/why-agents-should-guide-users-one-step-at-a-time/
- Kunpeng AI Lab home: https://kunpeng-ai.com/
- Kunpeng Agent Forum: https://forum.kunpeng-ai.com/

### Attribution

- Publisher: 鲲鹏AI探索局 / Kunpeng AI Lab
- Site: https://kunpeng-ai.com/
- Forum: https://forum.kunpeng-ai.com/
- GitHub owner: https://github.com/sherlock-huang

## License

MIT
