# Minimalist Entrepreneur Skills for OpenCode

OpenCode agent skills based on *The Minimalist Entrepreneur* by Sahil Lavingia. Frameworks for building a profitable, sustainable business starting from community.

Adapted from [slavingia/skills](https://github.com/slavingia/skills) (Claude Code format) into the [OpenCode skills format](https://opencode.ai/docs/skills/).

## Installation

Clone this repo into your project or home directory:

```bash
# Project-level (skills available in this project only)
git clone https://github.com/Adoit/minimalist-entrepreneur-skills.git
mkdir -p .opencode/skills
cp -r minimalist-entrepreneur-skills/.opencode/skills/* .opencode/skills/

# Or global (skills available in all projects)
mkdir -p ~/.config/opencode/skills
cp -r minimalist-entrepreneur-skills/.opencode/skills/* ~/.config/opencode/skills/
```

Or simply clone and work inside the repo -- OpenCode auto-discovers `.opencode/skills/*/SKILL.md` files.

## Skills

| Skill | Description | Stage |
|-------|-------------|-------|
| `find-community` | Identify and evaluate communities to build a business around | Ideation |
| `validate-idea` | Validate a business idea before building anything | Validation |
| `processize` | Turn an idea into a manual-first process you can deliver today | Validation |
| `mvp` | Build a minimum viable product -- manual first, then processized, then productized | Building |
| `pricing` | Figure out pricing using minimalist entrepreneur principles | Monetization |
| `first-customers` | Strategy for selling to your first 100 customers | Sales |
| `marketing-plan` | Build an audience through content, not ads | Marketing |
| `grow-sustainably` | Evaluate decisions for sustainable, profitable growth | Growth |
| `company-values` | Define company values and culture | Culture |
| `minimalist-review` | Gut-check any business decision through the minimalist lens | Evaluation |

## Usage

Once installed, OpenCode will list these skills in the `skill` tool description. The agent can load any skill on demand:

```
skill({ name: "validate-idea" })
```

Or you can ask the agent directly:

> "Help me validate my business idea using the minimalist entrepreneur framework"
> "I need to figure out pricing for my SaaS product"
> "Review my decision to hire two engineers through the minimalist entrepreneur lens"

The agent will automatically match your request to the relevant skill.

## Suggested Journey

These skills follow the stages of building a minimalist business:

1. **Find your community** (`find-community`) -- Start with people, not a product
2. **Validate your idea** (`validate-idea`) -- Test before you build
3. **Processize it** (`processize`) -- Deliver value manually first
4. **Build your MVP** (`mvp`) -- Ship the simplest thing that works
5. **Set your pricing** (`pricing`) -- Charge from day one
6. **Get your first customers** (`first-customers`) -- Sell one by one
7. **Create a marketing plan** (`marketing-plan`) -- Scale with content, not ads
8. **Grow sustainably** (`grow-sustainably`) -- Profitability is the goal
9. **Define your values** (`company-values`) -- Build the house you want to live in
10. **Review any decision** (`minimalist-review`) -- Apply the framework to anything

## Attribution

Based on *The Minimalist Entrepreneur* by Sahil Lavingia. Original Claude Code skills by [Sahil Lavingia](https://github.com/slavingia/skills).

## License

MIT
