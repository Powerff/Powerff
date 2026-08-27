# murphy

**Full-stack engineer** · production delivery · practical AI-assisted engineering

GitHub handle: [@Powerff](https://github.com/Powerff) · [Website](https://powerff.github.io/) · [eng-code-skills](https://github.com/Powerff/eng-code-skills)

---

I ship systems that hold up under deadlines, legacy constraints, and production risk — and I package the judgment that usually only lives in senior review into reusable **Agent Skills** for Cursor, Claude Code, and [agentskills.io](https://agentskills.io).

The aim is not flashy demos. It is **repeatable engineering quality**: clear scope, minimal diffs, explicit risks, and human ownership of release decisions.

| | |
| --- | --- |
| **Role** | Full-stack engineer |
| **Strength** | Backend contracts & safety · frontend state/effects · delivery discipline |
| **Open source** | [eng-code-skills](https://github.com/Powerff/eng-code-skills) — MIT Agent Skill suite (v0.2 · 24 skills) |
| **Languages** | 中文 · English |

---

## Focus

| Area | What I optimize for |
| --- | --- |
| **Delivery** | Clear scope, smallest viable diff, verify-before-merge |
| **Code quality** | Structure & readability without silent business-logic drift |
| **Backend** | API contracts, transactions, concurrency, resource lifecycle, data safety, layering (DTO/VO/Entity) |
| **Frontend** | State ownership, Hooks/effects hygiene, render cost, interaction correctness, component boundaries |
| **AI × Engineering** | Portable skills, checklists, phased workflows, human gates for irreversible decisions |

---

## Selected work

### [eng-code-skills](https://github.com/Powerff/eng-code-skills)

Open-source suite of **self-contained engineering Agent Skills** (MIT). Install one skill or the full set. Compatible with agentskills.io, Cursor, and Claude Code.

**v0.2 · 24 skills across four layers:**

| Layer | Coverage |
| --- | --- |
| **General** | Style check · safe refactor · tech-debt scan · code review |
| **Backend analysis** | Domain style / refactor / debt / review · **API layer (DTO/VO/Entity)** |
| **Backend workflows** | Coding standards · review-driven optimize · evidence-based bug fix · commit craft · implement–verify–(commit/restart) loops · project-level service refactor |
| **Frontend** | Domain style / refactor / debt / review · **Hooks check** · **component audit** · project-level migration |

**Design principles**

1. **Independence** — each skill folder is installable alone; no cross-skill file dependency  
2. **Domain separation** — general / backend / frontend rules stay distinct; no one-size-fits-all mega-prompt  
3. **Behavior preservation by default** — flag logic risks instead of “quietly fixing” them  
4. **Forced accountability** — every run should emit **risk warnings** and a **manual verification checklist**  
5. **Phased migration** — large refactors follow chain analysis → plan review → implement → CR → test loop

```bash
# Example: load a single skill
npx agentskills load github:Powerff/eng-code-skills#skills/backend-implement-verify-commit
npx agentskills load github:Powerff/eng-code-skills#skills/frontend-hooks-check
```

---

## Engineering stance

1. **AI accelerates; humans own the release.** Model output is advisory until reviewed, tested, and accepted.  
2. **Refactor ≠ line-by-line rewrite.** Cost sits in recovering rules buried in call chains, state machines, implicit validation, and historical patches — then re-expressing them in the target architecture.  
3. **Process beats a single mega-prompt.** Prefer phased work with human checkpoints, rollback paths, and cost caps (read / fix / test loops).  
4. **Domain failure modes differ.** Backend (consistency, locks, IO) and frontend (state, effects, UX regressions) need different checklists.  
5. **Evidence over vibes.** Prefer logs, diffs, builds, and reproducible paths over “should be equivalent.”

---

## Currently exploring

- Encoding team conventions as portable Skills / rules that survive chat context loss  
- Safe large-scale refactor workflows (ownership maps, GAP tables, clarification logs)  
- Practical harness patterns: validation loops, observability hooks, escalation when automation stalls  
- Writing for engineers: reproducible steps, trade-offs, and failure modes — not hype

---

## Toolbox

| Category | Tools & practices |
| --- | --- |
| **Languages & stacks** | Java / Spring · Go · TypeScript / JavaScript · React / Vue |
| **AI & workflow** | Agent Skills · Cursor · Claude Code · structured review & verify loops |
| **Engineering habits** | Incremental delivery · characterization before risky change · explicit risk surfacing · graph-oriented impact analysis when available |

---

## Contact

- GitHub: [@Powerff](https://github.com/Powerff)
- Website: [murphy.code](https://powerff.github.io/)
- Open source: [eng-code-skills](https://github.com/Powerff/eng-code-skills)

> **In one line:** Ship reliable software, and encode hard-won engineering judgment into tools others can run — with boundaries, verification, and clear ownership of risk.

---

## 中文简介

你好，我是 **murphy** —— **全栈工程师**，长期在真实交付约束下做工程落地，并持续把可复用的工程判断沉淀为 AI Agent Skills。

> GitHub 账号名为 [@Powerff](https://github.com/Powerff)（用户名 `murphy` / 域名 `murphy.github.io` 已被占用，故站点仍为 [powerff.github.io](https://powerff.github.io/)）。

### 我做什么

- **交付可靠系统**：在工期、遗留代码、评审标准与生产风险并存时，仍坚持小步改动、先验证后合入。  
- **把「会审代码的人」沉淀成工具**：将规范、评审、重构、排障、验证做成可安装的 **Agent Skills**，让 Cursor / Claude Code 按同一套标准执行，而不是每次从零口述规则。  
- **前后端都按失败模式设计检查清单**：后端关注契约、事务、并发、资源与数据安全；前端关注状态归属、Hooks/副作用、渲染成本与交互正确性。

### 代表开源

[eng-code-skills](https://github.com/Powerff/eng-code-skills)（MIT · v0.2 · **24** 个自包含技能）

| 分层 | 内容 |
| --- | --- |
| 通用 | 规范检查 · 安全重构 · 技术债务扫描 · 代码评审 |
| 后端分析 | 领域检查 / 重构 / 债务 / 评审 · **接口分层（DTO/VO/Entity）** |
| 后端工作流 | 编码规范 · 评审驱动优化 · 证据驱动修 Bug · 提交说明 · 实现–验证–（提交/重启）闭环 · 项目级服务重构 |
| 前端 | 领域检查 / 重构 / 债务 / 评审 · **Hooks 专项** · **组件审计** · 项目级迁移 |

**默认约束：** 不静默篡改业务语义；每次输出必须带 **风险警告** 与 **人工校验点**；大型重构走「链路分析 → 方案审查 → 编码 → CR → 测试闭环」。

### 原则

1. **AI 加速，人不让渡上线责任**  
2. **重构先梳清规则，再落目标架构** —— 成本在调用链与隐含约束，不在「搬运代码」  
3. **流程与证据优先于一次性神 Prompt** —— 分阶段、可回滚、可验证  

欢迎就工程落地、代码质量体系，以及 AI 协作的边界与方法论交流。
