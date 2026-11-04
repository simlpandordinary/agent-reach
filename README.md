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

>

## 目录结构

```
['SKILL.md', 'SKILL_en.md', 'references/capabilities.md', 'references/maintenance.md', 'references/sessions.md', 'agent_reach/__init__.py', 'agent_reach/backends/__init__.py', 'agent_reach/backends/boss_native.py', 'agent_reach/backends/cloak.py', 'agent_reach/backends/opencli.py', 'agent_reach/channels/__init__.py', 'agent_reach/channels/_opencli_site.py', 'agent_reach/channels/base.py', 'agent_reach/channels/bilibili.py', 'agent_reach/channels/boss.py', 'agent_reach/channels/facebook.py', 'agent_reach/channels/github.py', 'agent_reach/channels/instagram.py', 'agent_reach/channels/linkedin.py', 'agent_reach/channels/reddit.py', 'agent_reach/channels/twitter.py', 'agent_reach/channels/v2ex.py', 'agent_reach/channels/web.py', 'agent_reach/channels/xiaohongshu.py', 'agent_reach/channels/xiaoyuzhou.py', 'agent_reach/channels/xueqiu.py', 'agent_reach/channels/youtube.py', 'agent_reach/cli.py', 'agent_reach/config.py', 'agent_reach/runtime/__init__.py', 'agent_reach/runtime/bridge.py', 'agent_reach/runtime/browser.py', 'agent_reach/runtime/browser_binding.py', 'agent_reach/runtime/browser_watcher.py', 'agent_reach/runtime/cdp.py', 'agent_reach/runtime/cli.py', 'agent_reach/runtime/clock.py', 'agent_reach/runtime/dispatch.py', 'agent_reach/runtime/legacy.py', 'agent_reach/runtime/manage.py', 'agent_reach/runtime/onboarding.py', 'agent_reach/runtime/public_web.py', 'agent_reach/runtime/result.py', 'agent_reach/runtime/run.py', 'agent_reach/runtime/session_reuse.py', 'agent_reach/runtime/sessions.py', 'agent_reach/runtime/state.py', 'agent_reach/runtime/tools.py', 'agent_reach/runtime/update_notice.py', 'agent_reach/scripts/transcribe_xiaoyuzhou.sh', 'agent_reach/transcribe.py', 'agent_reach/utils/paths.py', 'agent_reach/utils/process.py', 'agent_reach/utils/text.py', 'agent_reach/utils/url.py', 'scripts/accept-search.py', 'scripts/check_release_acceptance.py', 'scripts/record_release_acceptance.py', 'pyproject.toml', 'constraints.txt', 'llms.txt', 'README.upstream.md', 'LICENSE']
```

- `SKILL.md` 是技能入口（触发条件 / 工作流 / 约束），安装时必须位于技能根目录。
- `references/`、`scripts/`、`assets/` 为该技能自带的参考文档、脚本与素材。
- `README.upstream.md` 为上游仓库原始说明，保留出处与版权信息。
- `LICENSE` 为上游许可证原文。

## 安装

WorkBuddy 技能目录为 `~/.workbuddy/skills/agent-reach/`：

```bash
git clone https://github.com/simlpandordinary/agent-reach.git ~/.workbuddy/skills/agent-reach
```

也可以直接对 AI 说：「把 <https://github.com/simlpandordinary/agent-reach> 装成 Skill」。

安装后用自然语言触发，例如「Agent-Reach（给 AI 装眼睛）」「用 agent-reach 帮我处理这个任务」。



## 版权

原始作者与版权归上游仓库 `Panniantong/Agent-Reach` 所有。本仓库仅做独立分发与结构整理，未修改技能内容；商用请遵循上游许可证。
