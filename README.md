# Agent-Reach（给 AI 装眼睛）

> **[agent-reach](https://github.com/simlpandordinary/agent-reach)** —— 飞书《WorkBuddy 视频系列 · 全技能与提示词总目录》里推荐的开源技能，已拆分为独立仓库分发（一个技能一个仓库）。

| 项 | 内容 |
| - | - |
| 上游仓库 | <https://github.com/Panniantong/Agent-Reach> |
| 上游路径 | `agent_reach/skill` |
| 上游协议 | MIT |
| 上游 Star | 108k+ |
| 拆分方式 | 仅抽取该技能自身文件，独立可用 |

## 技能说明

只读读取各平台内容：搜索、读帖、看评论、取字幕、查行情和职位。 Use when 用户提到或贴出链接：小红书/xiaohongshu、B站/bilibili、Twitter/X、Reddit、 YouTube（字幕、转录）、GitHub、V2EX、雪球/股票行情、LinkedIn/Boss直聘 职位、 Instagram、Facebook、小宇宙播客；或说"帮我搜/看看/读一下这个链接"而自带网页搜索/读取不可用、失败或拿不到正文； 或要安装、加上/去掉某个平台、登录/退出、看状态、更新、卸载 Agent Reach。 不做：发帖、评论、点赞、私信等任何写操作；不替用户登录、不索要密码。 公开内容优先用 Agent 自带工具，Reach 补缺口。

## 目录结构

```
├── LICENSE
├── README.upstream.md
├── SKILL.md
├── SKILL_en.md
├── constraints.txt
├── llms.txt
├── pyproject.toml
├── scripts/
│   ├── accept-search.py
│   ├── check_release_acceptance.py
│   └── record_release_acceptance.py
├── references/
│   ├── capabilities.md
│   ├── maintenance.md
│   └── sessions.md
└── agent_reach/
    ├── __init__.py
    ├── cli.py
    ├── config.py
    ├── transcribe.py
    ├── utils/
    │   ├── paths.py
    │   ├── process.py
    │   ├── text.py
    │   └── url.py
    ├── scripts/
    │   └── transcribe_xiaoyuzhou.sh
    ├── runtime/
    │   ├── __init__.py
    │   ├── bridge.py
    │   ├── browser.py
    │   ├── browser_binding.py
    │   ├── browser_watcher.py
    │   ├── cdp.py
    │   ├── cli.py
    │   ├── clock.py
    │   ├── dispatch.py
    │   ├── legacy.py
    │   ├── manage.py
    │   ├── onboarding.py
    │   ├── public_web.py
    │   ├── result.py
    │   ├── run.py
    │   ├── session_reuse.py
    │   ├── sessions.py
    │   ├── state.py
    │   ├── tools.py
    │   └── update_notice.py
    ├── channels/
    │   ├── __init__.py
    │   ├── _opencli_site.py
    │   ├── base.py
    │   ├── bilibili.py
    │   ├── boss.py
    │   ├── facebook.py
    │   ├── github.py
    │   ├── instagram.py
    │   ├── linkedin.py
    │   ├── reddit.py
    │   ├── twitter.py
    │   ├── v2ex.py
    │   ├── web.py
    │   ├── xiaohongshu.py
    │   ├── xiaoyuzhou.py
    │   ├── xueqiu.py
    │   └── youtube.py
    └── backends/
        ├── __init__.py
        ├── boss_native.py
        ├── cloak.py
        └── opencli.py
```

- `SKILL.md` 是技能入口（触发条件 / 工作流 / 约束），安装时必须位于技能根目录。
- `references/`、`scripts/`、`assets/` 为该技能自带的参考文档、脚本与素材。
- `README.upstream.md` 为上游仓库原始说明，保留出处与版权信息。
- `LICENSE` 为上游许可证原件。

## 安装

WorkBuddy 技能目录为 `~/.workbuddy/skills/agent-reach/`：

```bash
git clone https://github.com/simlpandordinary/agent-reach.git ~/.workbuddy/skills/agent-reach
```

也可以直接对 AI 说：「把 <https://github.com/simlpandordinary/agent-reach> 装成 Skill」。

安装后用自然语言触发，例如「Agent-Reach（给 AI 装眼睛）」「用 agent-reach 帮我处理这个任务」。

## 版权

原始作者与版权归上游仓库 `Panniantong/Agent-Reach` 所有。本仓库仅做独立分发与结构整理，未修改技能内容；商用请遵循上游许可证。
