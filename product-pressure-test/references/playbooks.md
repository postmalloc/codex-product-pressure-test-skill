# Product Pressure Test Playbooks

Use these playbooks when the user requests a specific mode or a deep/full evaluation.

## Fit Check

Role:

Act as a senior product strategy evaluator deciding whether a product idea deserves resources inside the user's company.

Task:

Evaluate whether the idea fits the company's current business, customers, products, distribution, assets, constraints, and operating model.

Steps:

- Ask for company context if missing.
- Identify the existing business or product surface the idea attaches to.
- Identify reused assets: customers, data, distribution, trust, workflows, integrations, domain expertise, brand, sales motion.
- Identify mismatches: new ICP, new buyer, new support burden, new regulatory exposure, new technical platform, channel conflict.
- Determine the company's right to win.
- Give a direct verdict: build, pilot, park, or pivot required.

Rules:

- Fit is not "the company could build it"; fit means the company has a credible advantage and adoption path.
- A product that needs a new ICP, new GTM, new support model, and new technical stack is effectively a new business.
- A weak fit can still be worth an internal-tool pilot if it reduces a clear operating cost.

Output:

- Company Context Gaps
- Current Business Link
- Reused Assets
- Fit Mismatches
- Right To Win
- Verdict

## Problem Validation

Role:

Act as a product discovery lead testing whether the problem is real for the company's current or adjacent users.

Task:

Validate whether the idea solves a painful, frequent, valuable job for real users/customers, or whether it is an internal wish dressed up as product strategy.

Steps:

- Ask for target user/customer if missing.
- Define the specific job, trigger, pain, frequency, and consequence.
- Identify who has the problem most acutely in the company's current customer base or user base.
- Identify evidence the company already has: support tickets, churn notes, sales objections, usage logs, CRM notes, NPS verbatims, manual workarounds.
- Write discovery questions that reveal past behavior without leading the witness.
- Define validation criteria: what evidence proves the problem is urgent enough to build for.

Rules:

- Questions must ask about past behavior, not hypothetical intent.
- Segment by current customers, adjacent customers, internal teams, and non-customers when relevant.
- Validate willingness to change workflow, pay, expand contract, reduce churn, or allocate time.

Good questions:

- "What did you do the last time this happened?"
- "Which tool or manual process did you use instead?"
- "How often does this happen, and what does it cost?"
- "Who else gets pulled in when this breaks?"
- "What would make this worth switching from the current workflow?"

Bad questions:

- "Would you use this?"
- "Would your team like this?"
- "Should we add this feature?"

Output:

- Specific Job/Pain
- Best-Fit Segment
- Existing Evidence To Mine
- Discovery Questions
- Validation Criteria
- Painkiller/Vitamin Verdict

## Strategy Alignment

Role:

Act as a product executive evaluating whether the idea advances the company's strategy instead of just expanding the roadmap.

Task:

Assess whether the idea materially supports company goals such as revenue, retention, expansion, differentiation, efficiency, risk reduction, platform leverage, or strategic positioning.

Steps:

- Ask for company goals or OKRs if missing.
- Map the idea to one or two concrete outcomes.
- Identify whether the idea strengthens the core product, creates an expansion path, defends retention, opens a new segment, or reduces operating cost.
- Check whether it conflicts with positioning, sales motion, pricing, roadmap focus, or customer expectations.
- Define measurable strategic impact and time horizon.

Rules:

- "Strategic" must map to a measurable business outcome.
- Avoid ideas that create complexity without meaningful leverage.
- Do not let novelty substitute for focus.

Output:

- Strategic Outcome
- Link To Current Goals
- Upside Case
- Focus/Complexity Cost
- Strategic Fit Verdict

## Status Quo Map

Role:

Act as a competitive and workflow analyst. The most dangerous competitor is often the current workflow.

Task:

Map what users, customers, and internal teams do today instead of using the proposed product.

Steps:

- Ask for the target workflow if missing.
- Identify current internal process, spreadsheet, vendor, workaround, manual service, adjacent feature, or no-action behavior.
- Map direct competitors and product substitutes.
- Map internal alternatives the company could ship instead.
- Assess switching cost: data migration, retraining, procurement, approvals, workflow disruption, trust, compliance, habit.
- Identify the real enemy: status quo, vendor lock-in, budget owner, implementation burden, or lack of urgency.

Rules:

- "No competition" is always wrong.
- Status quo wins unless the new product is meaningfully better on a job that matters.
- Differentiation must be specific to the company's right to win.

Output:

- Current Workflow
- Direct Alternatives
- Internal Alternatives
- Real Enemy
- Switching Cost
- Differentiation Needed

## Stakeholder Adoption

Role:

Act as a product operator mapping the incentives and blockers required for adoption inside a company ecosystem.

Task:

Identify who must care, approve, use, sell, operate, support, integrate, and maintain the product for it to work.

Steps:

- Separate user, buyer, approver, admin, operator, support team, sales team, compliance/security, and technical owner.
- Map what each stakeholder gains, loses, or fears.
- Identify adoption blockers: training, workflow change, sales enablement, pricing, support load, data permissions, implementation effort.
- Define launch path: internal pilot, customer design partner, beta cohort, existing package add-on, enterprise upsell, self-serve feature, or partner integration.
- Identify the adoption metric that matters.

Rules:

- A product can fail even when users like it if buyers, operators, sales, or support teams are misaligned.
- Watch for products that create cost in one team while value accrues to another.

Output:

- Stakeholder Map
- Incentives
- Adoption Blockers
- Launch Path
- Adoption Metric

## MVP Pilot

Role:

Act as an MVP architect for an established company. The goal is to test the riskiest assumption without committing full roadmap capacity.

Task:

Design the smallest credible pilot that tests whether the idea fits the company's users, business, and operating model.

Steps:

- Identify the single riskiest assumption.
- Choose the pilot audience: internal team, customer design partner, beta cohort, existing account segment, or shadow-mode workflow.
- Define the minimum scope needed to test behavior.
- Cut every feature that does not test the assumption.
- Define instrumentation, success metric, failure threshold, and decision date.
- Define what happens after pass/fail.

Rules:

- A pilot must reach real users or real internal operators, not only internal demos.
- Prefer concierge, manual, prototype, or integration-light tests when they expose the core risk faster.
- Success criteria must be behavioral: usage, paid expansion, retention signal, workflow replacement, cost reduction, cycle time reduction, support deflection, or risk reduction.

Output:

- Riskiest Assumption
- Pilot Audience
- Minimum Scope
- What Gets Cut
- Success/Failure Criteria
- Next Decision

## Build-Buy-Partner

Role:

Act as a pragmatic product and strategy advisor deciding whether the company should build the idea itself.

Task:

Compare build, buy, partner, integrate, or avoid paths based on strategic importance, speed, cost, differentiation, operational burden, and risk.

Steps:

- Identify whether the capability is core differentiation or table stakes.
- Assess available internal expertise and technical leverage.
- Identify vendor/partner alternatives and integration options.
- Compare speed to learning versus speed to full launch.
- Consider ownership, compliance, data control, support, maintenance, and switching costs.
- Recommend the path that best tests or captures the opportunity.

Rules:

- Build when the capability is strategically differentiating and the company has a right to win.
- Buy or partner when the capability is table stakes, commodity, or faster to validate externally.
- Avoid when the idea is off-strategy and lacks urgent pain.

Output:

- Core vs Commodity
- Build Case
- Buy/Partner Case
- Key Risks
- Recommendation
