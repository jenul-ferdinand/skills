# Agent Skills

[Agent Skills](https://agentskills.io) I've built, packaged as a Claude Code plugin marketplace. Each skill lives in its own repo, linked here under `plugins/`.

| Skill | What it does |
| --- | --- |
| [cashew-skill](https://github.com/jenul-ferdinand/cashew-skill) | Tell your agent what you spent, and it lands in [Cashew](https://github.com/jameskokoska/Cashew), the open-source budgeting app. |
| [etoro-skill](https://github.com/jenul-ferdinand/etoro-skill) | Your agent reads your live [eToro](https://www.etoro.com) balance, holdings and P/L before answering questions about your investments. Read-only. |

## Install

In Claude Code, add the marketplace once, then install what you want:

```
/plugin marketplace add jenul-ferdinand/skills
/plugin install etoro-skill@jenul-skills
/plugin install cashew-skill@jenul-skills
```

For other agents, install a skill straight from its repo, for example `npx skills add jenul-ferdinand/etoro-skill -g`. Each skill's README covers its setup.

The `plugins/` folders are git submodules that point at each skill's repo. Installs fetch from those repos directly, so you always get the latest version.

Unofficial, and not affiliated with Cashew or eToro. MIT licensed.
