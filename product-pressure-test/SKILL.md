---
name: product-pressure-test
description: Validate and pressure-test product ideas to build inside an existing company. Use when Codex is asked to evaluate whether a product idea fits a company's current business, customers, products, strategy, assets, constraints, roadmap, go-to-market motion, or internal adoption path; define discovery questions, stakeholder risks, MVP/pilot scope, build-buy-partner options, or give a direct build/pilot/park/pivot verdict.
---

# Product Pressure Test

## Overview

Use this skill to pressure-test product ideas that would be built within an existing company. Evaluate the idea against the company's current business, customers, distribution, data, technical stack, operating model, and strategic goals. Be direct, specific, and practical: the goal is to decide whether the idea deserves discovery, a pilot, a build slot, or a kill/pivot.

## Language

Match the user's language. If the user writes in Italian, answer in Italian. If the user writes in English, answer in English. Keep common product terms in English when clearer: `ICP`, `MVP`, `PMF`, `JTBD`, `OKR`, `GTM`, `pilot`, `stakeholder`, `right to win`.

## First Move

If the idea is missing, ask for it first:

```text
Send me the product idea, what the company does today, target users/customers, and the business outcome you want.
```

If the idea is present but company context is thin, ask focused company-context questions before giving a verdict:

1. What does the company do or sell today, and to whom?
2. How does it make money or measure success?
3. What current products, workflows, data, channels, or customer relationships could this idea reuse?
4. Which users, buyers, approvers, operators, or support teams would need to adopt or sustain it?
5. What constraints matter: roadmap, tech stack, regulation, brand, sales motion, budget, or timeline?

If the user asks for a quick pass without answering, proceed with explicit assumptions and mark confidence as low.

## Modes

Choose the mode from the user request. If unclear, use `full`.

- `fit-check`: evaluate whether the idea fits the company's business, assets, customers, strategy, and operating model.
- `problem-validation`: test whether the user/customer pain is real, frequent, urgent, and already causing behavior.
- `strategy-alignment`: assess whether the idea advances company goals, moat, retention, revenue, cost reduction, or risk reduction.
- `status-quo-map`: map current workflows, internal substitutes, vendors, competitors, and switching costs.
- `stakeholder-adoption`: identify buyer/user/approver/operator incentives and adoption blockers.
- `mvp-pilot`: define the smallest pilot that tests the riskiest assumption with real users or customers.
- `build-buy-partner`: decide whether the company should build, buy, partner, integrate, or avoid the idea.
- `full`: run a compact version of all modes.

Read `references/playbooks.md` for the detailed criteria and output templates for each mode.

## Default Output

Default to compact output. Most users need a sharp decision memo they can scan quickly, not a long essay. Include the scorecard by default.

Use this shape:

```markdown
**Verdict**
Build / Pilot / Park / Pivot required

2-3 direct sentences.

**Scorecard**
| Area | Score | Read |
|---|---:|---|
| Company fit | 3/5 | ... |
| User/customer pain | 2/5 | ... |
| Business impact | 4/5 | ... |
| Strategic alignment | 3/5 | ... |
| Adoption path | 2/5 | ... |
| Feasibility/speed | 4/5 | ... |

**Core Assumption**
One sentence.

**Company Fit**
- Current business link: ...
- Reused asset/channel/data: ...
- Right to win: ...

**Fatal Flaws**
| Risk | Severity | Why It Matters | Fast Test |
|---|---|---|---|
| ... | High | ... | ... |

**User/Customer Reality**
- Pain/job: ...
- Current behavior: ...
- Who must change behavior: ...

**Status Quo And Alternatives**
- Current workflow: ...
- Internal or vendor alternative: ...
- Switching cost: ...

**Pilot**
- Build:
- Cut:
- Success metric:
```

Default limits:

- Scorecard: always include 6 rows.
- Verdict: max 3 sentences.
- Company Fit: max 3 bullets.
- Fatal Flaws: max 3 rows.
- User/Customer Reality: max 3 bullets.
- Status Quo And Alternatives: max 3 bullets.
- Pilot: max 3 bullets.
- Do not include long research plans, PRDs, roadmaps, or discovery scripts unless the user asks for more detail.

## Rules

- Start from the company as it exists today, not the idea in isolation.
- Be specific to the company's business, users, channels, assets, constraints, and current products.
- Separate user, buyer, approver, implementer, operator, and support incentives when they differ.
- Identify the core assumption that must be true for the product to deserve company resources.
- Treat current behavior, internal processes, spreadsheets, agencies, vendors, and existing product surfaces as competition.
- Treat "we can just add it" as false until adoption, ownership, support, and GTM are credible.
- Test behavior, not compliments: usage logs, tickets, churn reasons, sales objections, support cost, manual workarounds, paid pilots, or workflow change.
- Pressure-test strategic fit: revenue, retention, expansion, cost reduction, risk reduction, moat, brand, and focus.
- Flag cannibalization, channel conflict, privacy/security, regulatory, operational, support, and maintenance risks.
- Prefer the smallest pilot that tests the riskiest assumption before committing roadmap capacity.
- If the idea fits poorly, say so directly and suggest a narrower adjacent use case, internal tool path, partner path, or kill criteria.
- Do not invent fake market data. If current market facts matter and are uncertain, browse or state what must be verified.

## Scoring

Use scores only when useful:

| Area | Score |
|---|---:|
| Company fit | 1-5 |
| User/customer pain | 1-5 |
| Business impact | 1-5 |
| Strategic alignment | 1-5 |
| Adoption path | 1-5 |
| Feasibility/speed | 1-5 |

Scores must be tied to evidence from the idea and company context, not vibes.

## Deep Mode

If the user asks for `deep`, `full report`, `brutal`, `be extremely honest`, or `give me more detail`, expand each section with:

- assumptions to validate
- disconfirming evidence to look for
- company-context questions
- customer or internal discovery questions
- stakeholder map
- pilot design and instrumentation
- build-buy-partner recommendation
- decision memo with kill criteria

Still keep the writing direct and structured.

## Resources

- `references/playbooks.md`: Mode-specific checklists and output details.
