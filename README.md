# Minimalist Entrepreneur Skills for OpenCode

OpenCode agent skills based on *The Minimalist Entrepreneur* by Sahil Lavingia. Frameworks for building a profitable, sustainable business starting from community.

Adapted from [slavingia/skills](https://github.com/slavingia/skills) (Claude Code format) into the [OpenCode skills format](https://opencode.ai/docs/skills/).

## Installation

Clone this repo into your project or home directory:

```bash
# Project-level (skills + commands available in this project only)
git clone https://github.com/Adoit/minimalist-entrepreneur-skills.git
mkdir -p .opencode/skills .opencode/commands
cp -r minimalist-entrepreneur-skills/.opencode/skills/* .opencode/skills/
cp -r minimalist-entrepreneur-skills/.opencode/commands/* .opencode/commands/

# Or global (skills + commands available in all projects)
mkdir -p ~/.config/opencode/skills ~/.config/opencode/commands
cp -r minimalist-entrepreneur-skills/.opencode/skills/* ~/.config/opencode/skills/
cp -r minimalist-entrepreneur-skills/.opencode/commands/* ~/.config/opencode/commands/
```

Or simply clone and work inside the repo -- OpenCode auto-discovers `.opencode/skills/*/SKILL.md` and `.opencode/commands/*.md` files.

## Skills

| Skill | Command | Description | Stage |
|-------|---------|-------------|-------|
| `find-community` | `/find-community` | Identify and evaluate communities to build a business around | Ideation |
| `validate-idea` | `/validate-idea` | Validate a business idea before building anything | Validation |
| `processize` | `/processize` | Turn an idea into a manual-first process you can deliver today | Validation |
| `mvp` | `/mvp` | Build a minimum viable product -- manual first, then processized, then productized | Building |
| `pricing` | `/pricing` | Figure out pricing using minimalist entrepreneur principles | Monetization |
| `first-customers` | `/first-customers` | Strategy for selling to your first 100 customers | Sales |
| `marketing-plan` | `/marketing-plan` | Build an audience through content, not ads | Marketing |
| `grow-sustainably` | `/grow-sustainably` | Evaluate decisions for sustainable, profitable growth | Growth |
| `company-values` | `/company-values` | Define company values and culture | Culture |
| `minimalist-review` | `/minimalist-review` | Gut-check any business decision through the minimalist lens | Evaluation |

## Usage

### Slash Commands

The quickest way to use these skills is via slash commands. Type `/` in the OpenCode TUI:

```
/pricing my SaaS product for freelance designers
/validate-idea a tool that helps podcasters find guests
/minimalist-review should I hire a contractor or use no-code tools?
/find-community
/mvp
```

Commands accept optional arguments. If you omit them, the agent will ask clarifying questions.

### Natural Language

You can also just ask naturally -- the agent will match your request to the right skill automatically:

> "Help me validate my business idea using the minimalist entrepreneur framework"
> "I need to figure out pricing for my SaaS product"
> "Review my decision to hire two engineers through the minimalist entrepreneur lens"

### Programmatic (skill tool)

The agent can also load skills directly via the built-in `skill` tool:

```
skill({ name: "validate-idea" })
```

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
