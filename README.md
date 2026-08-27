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

你好，我是 **murphy** —— **Full-stack Engineer**。

面向生产交付：在真实工期、遗留约束与上线风险下交付可运行系统；把评审、重构、验证与分层规范沉淀为可安装的 **Agent Skills**，供 Cursor / Claude Code 及主流编码模型按同一套工程标准协作。

> GitHub：[@Powerff](https://github.com/Powerff) · 站点：[powerff.github.io](https://powerff.github.io/)

| | |
| --- | --- |
| **Domain** | Backend contracts · Frontend state/effects · Delivery discipline |
| **Open source** | [eng-code-skills](https://github.com/Powerff/eng-code-skills) · [codebase-agent-kit](https://github.com/Powerff/codebase-agent-kit) |
| **Operating rule** | 不静默改业务语义 · 风险显性化 · 人工闸门负责上线 |

### 代表开源

[eng-code-skills](https://github.com/Powerff/eng-code-skills)（MIT · v0.2.2 · **25** 个自包含技能）

| 分层 | 内容 |
| --- | --- |
| 通用 | 规范检查 · 安全重构 · 技术债务扫描 · 代码评审 |
| 后端分析 | 领域检查 / 重构 / 债务 / 评审 · **接口分层（DTO/VO/Entity）** |
| 后端工作流 | 编码规范 · 优化 · 修 Bug · 提交 · 实现–验证–（提交/重启） · 服务重构 · **技术栈升级（JDK 等）** |
| 前端 | 领域检查 / 重构 / 债务 / 评审 · **Hooks 专项** · **组件审计** · 项目级迁移 |

**模式：** 分析类默认只出报告/方案；工作流类会改工作区；仅 `backend-implement-verify-commit` / `backend-code-commit` 默认提交。详见 [Plan-only vs writes](https://github.com/Powerff/eng-code-skills#plan-only-vs-writes-to-your-repo)。

[codebase-agent-kit](https://github.com/Powerff/codebase-agent-kit)（MIT · v0.1 · **8** 个代码库级技能）

| 分层 | 内容 |
| --- | --- |
| 通用 | 项目上下文 · 跨文件重构 · 全仓债务审计 · 框架迁移方案 |
| 后端 | 全局风险审计 · 单体模块拆分 |
| 前端 | 全局风险审计 · 组件/模块拆分 |

**模式：全部只出方案，不覆盖仓库。** 落地请接 eng-code-skills 工作流（如 `backend-stack-upgrade`）。

**组合用法：** kit 定全局方案 → eng 工作流改码验证 → eng 分析类做单文件质量收尾。

**默认约束：** 不静默篡改业务语义；每次输出必须带 **风险警告** 与 **人工校验点**；大型重构走「链路分析 → 方案审查 → 编码 → CR → 测试闭环」。

### 原则

1. **AI 加速，人不让渡上线责任**  
2. **重构先梳清规则，再落目标架构** —— 成本在调用链与隐含约束，不在「搬运代码」  
3. **流程与证据优先于一次性神 Prompt** —— 分阶段、可回滚、可验证  

欢迎就工程落地、代码质量体系，以及 AI 协作的边界与方法论交流。
