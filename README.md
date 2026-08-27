# murphy · Powerff

**Full-stack engineer** focused on production delivery and practical AI-assisted engineering.

GitHub: [Powerff](https://github.com/Powerff) · Site: [murphy.code](https://powerff.github.io/murphy.code.github.io/)

I build systems that ship — and turn repeated engineering judgment into reusable **Agent Skills** for tools like Cursor and Claude Code. The goal is not clever demos; it is **repeatable quality** under real constraints: deadlines, legacy code, review standards, and production risk.

---

## Focus

| Area | What I care about |
| --- | --- |
| Delivery | Clear scope, minimal diffs, verify-before-merge discipline |
| Code quality | Structure and readability without silent business-logic drift |
| Backend | Contracts, transactions, concurrency, resource lifecycle, data safety |
| Frontend | State ownership, controlled effects, render cost, interaction correctness |
| AI × Engineering | Skills, checklists, phased workflows, human gates for irreversible decisions |

---

## Selected work

### [eng-code-skills](https://github.com/Powerff/eng-code-skills)

An open-source suite of **self-contained engineering Agent Skills** (MIT), compatible with [agentskills.io](https://agentskills.io), Cursor, and Claude Code.

**Coverage (21 skills):**

- **General** — style check, safe refactor, tech-debt scan, code review
- **Backend analysis** — backend-specific style / refactor / debt / review
- **Backend workflows** — coding standards, review-driven optimize, bug localization, commit craft, implement–verify loops
- **Frontend** — frontend-specific style / refactor / debt / review
- **Project refactor** — five-phase migration for backend & frontend (chain analysis → plan review → implement → CR → test loop)

**Design principles:**

1. Install one skill or the full set — each package is independent  
2. Separate general / backend / frontend rules — no one-size-fits-all prompts  
3. Default to **behavior preservation**; flag logic risks instead of “quietly fixing” them  
4. Every run should emit **risk warnings** and a **manual verification checklist**

---

## Engineering stance on AI coding

1. **AI accelerates; humans own the release.** Suggestions are advisory until reviewed and tested.  
2. **Refactor ≠ line-by-line rewrite.** Cost sits in recovering rules buried in call chains, state machines, implicit validation, and historical patches — then re-expressing them in the target architecture.  
3. **Process beats a single mega-prompt.** Prefer phased work with human checkpoints, rollback, and cost caps (read/fix/test loops).  
4. **Domain matters.** Backend failure modes (consistency, locks, IO) and frontend failure modes (state, effects, UX regressions) need different checklists.  
5. **Evidence over vibes.** Prefer logs, diffs, builds, and reproducible paths over “should be equivalent.”

---

## What I’m exploring

- Turning team conventions into portable Skills / rules that survive chat context loss  
- Safe large-scale refactor workflows (ownership maps, GAP tables, clarification logs)  
- Practical harness patterns: validation loops, observability hooks, escalation when automation stalls  
- Writing for engineers: reproducible steps, trade-offs, and failure modes — not hype

---

## Toolbox

**Languages & stacks:** Java / Spring · Go · TypeScript / JavaScript · React / Vue  

**AI & workflow:** Agent Skills · Cursor · Claude Code · structured review & verify loops  

**Practices:** incremental delivery · characterization before risky change · explicit risk surfacing

---

## Contact / links

- GitHub: [@Powerff](https://github.com/Powerff)
- Web: [powerff.github.io/murphy.code.github.io](https://powerff.github.io/murphy.code.github.io/)
- Project: [eng-code-skills](https://github.com/Powerff/eng-code-skills)

---

### Summary

> Ship reliable software, and encode the hard-won engineering judgment into tools other people can run — with boundaries, verification, and clear ownership of risk.

---

## 中文简介

你好，我是 **murphy（Powerff）**：全栈工程师，也在真实项目里使用 AI。

我关注把「规范、评审、重构、排障、验证」沉淀成可安装的 **Agent Skills**，让 Cursor / Claude Code 按同一套工程标准执行，而不是每次从零口述规则。

代表仓库：[eng-code-skills](https://github.com/Powerff/eng-code-skills) — 通用 / 后端 / 前端分层，支持单技能安装；默认不偷改业务语义；输出必须带风险警告与人工校验点。项目级重构技能采用「链路分析 → 方案审查 → 编码 → CR → 测试闭环」五阶段流程。

**原则：** AI 加速，人不让渡上线责任；重构先梳规则再落架构；流程与证据优先于一次性神 Prompt。

欢迎交流工程落地与 AI 协作实践。
