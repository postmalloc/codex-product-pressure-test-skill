# Codex Product Pressure Test Skill

A Codex skill to pressure-test product ideas before a company commits roadmap capacity to the wrong thing.

This package is an adaptation of the [Codex Startup Pressure Test Skill](https://github.com/Kappaemme-git/codex-startup-pressure-test-skill), refocused from startup idea validation to product ideas built inside an existing company.

Give Codex a product idea plus company context and it returns a compact product strategy diagnosis: verdict, scorecard, core assumption, company fit, fatal flaws, user/customer reality, status quo, adoption risks, and a pilot direction.

## What It Does

- Asks what the company does today before judging the idea
- Evaluates fit with current products, customers, channels, data, and strategy
- Exposes fatal product, adoption, operational, and GTM risks
- Checks whether the user/customer problem is real
- Maps status quo workflows, competitors, vendors, and internal substitutes
- Identifies stakeholder adoption blockers
- Defines the smallest pilot or MVP test
- Gives a direct build / pilot / park / pivot verdict

## Installation

```bash
npx --yes codex-product-pressure-test-skill@latest
```

This installs the skill into:

```bash
~/.codex/skills/product-pressure-test
```

Then restart Codex so it can discover the skill.

## Usage

After installation, restart Codex and use the skill inside Codex prompts.

Basic pressure test:

```text
Use $product-pressure-test to pressure-test this product idea for our company:

Company: We sell workflow software to mid-market accounting teams.
Idea: Add an AI assistant that drafts month-end close variance explanations.
Goal: Increase retention and expansion in accounts with complex close processes.
```

Fit check:

```text
Use $product-pressure-test to evaluate whether this product idea fits what our company does today:

...
```

Problem validation:

```text
Use $product-pressure-test to validate whether this idea solves a real customer problem:

...
```

Stakeholder adoption:

```text
Use $product-pressure-test to map adoption blockers and stakeholders for this product idea:

...
```

MVP/pilot plan:

```text
Use $product-pressure-test to design the smallest pilot for this idea:

...
```

Build-buy-partner:

```text
Use $product-pressure-test to decide whether we should build, buy, partner, or avoid this capability:

...
```

Deep report:

```text
Use $product-pressure-test to do a deep full report on this product idea for our company:

...
```

If you invoke the skill without enough context, it will ask what the company does today, who it serves, how it measures success, what assets the idea can reuse, who must adopt it, and what constraints matter.

## Modes

- `fit-check`: company fit, reused assets, right to win
- `problem-validation`: real pain, current behavior, validation criteria
- `strategy-alignment`: business outcome, focus cost, strategic fit
- `status-quo-map`: current workflow, alternatives, switching cost
- `stakeholder-adoption`: user/buyer/operator incentives and blockers
- `mvp-pilot`: smallest pilot with success/failure criteria
- `build-buy-partner`: build, buy, partner, integrate, or avoid
- `full`: compact all-in-one diagnosis

## Output

Default output is compact:

```text
Verdict
Scorecard
Core Assumption
Company Fit
Fatal Flaws
User/Customer Reality
Status Quo And Alternatives
Pilot
```

## Development

Validate the package locally:

```bash
node scripts/install.js --skills-dir /tmp/codex-product-pressure-test-skills
npm pack --dry-run
```

Publish to npm:

```bash
npm login
npm publish --access public
```

## Manual Installation

Clone the repository:

```bash
git clone https://github.com/Kappaemme-git/codex-product-pressure-test-skill.git
```

Copy the skill into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R codex-product-pressure-test-skill/product-pressure-test ~/.codex/skills/product-pressure-test
```

Restart Codex.

## Troubleshooting

If Codex does not recognize `$product-pressure-test`, restart Codex after installing.

Check that the skill exists:

```bash
ls ~/.codex/skills/product-pressure-test
```

You should see:

```text
SKILL.md
agents/
references/
```

## License

MIT
