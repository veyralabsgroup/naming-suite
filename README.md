# naming-suite

Four skills for naming products, auditing brands, mapping competitors, and building naming systems. Works with Claude Code and other AI coding agents.

```bash
npx @veyralabs/skills install naming-suite
```

---

## Skills

### domainforge

Generates startup name candidates and scores each one across 8 factors: memorability, distinctiveness, domain availability, trademark risk, pronunciation, spelling, brandability, and market fit. Returns a ranked list with domain availability, social handle checks, and a one-line brand narrative for each name.

### brandaudit

Audits an existing brand name. Analyzes it across 8 dimensions, assigns severity scores to each issue, and returns a verdict: keep, refine, or rebrand. Useful before launching a product or after a pivot.

### competitornames

Maps how competitors in a given market are named. Identifies naming clusters (what patterns dominate), saturation levels, and open whitespace. Produces a brief you can feed directly into domainforge.

### namingguide

Builds a complete naming system for a company or product line. Covers naming principles, approved patterns, anti-patterns, examples, and an approval checklist. Useful when a company is scaling and needs consistent naming across features, products, and teams.

---

## Recommended flow

```
competitornames  →  domainforge    (find a name)
brandaudit       →  namingguide    (fix and systematize an existing name)
```

Run `competitornames` first to understand what names already exist in your space. Then `domainforge` generates names that stand out from that landscape rather than blending in.

---

## Install

```bash
# Install the full pack
npx @veyralabs/skills install naming-suite

# Install a single skill
npx @veyralabs/skills install domainforge
```

### Manual

Copy the skill folder into your agent's skills directory:

| Agent | Path |
|-------|------|
| Claude Code | `.claude/skills/` |
| Cursor | `.cursor/skills/` |
| Windsurf | `.windsurf/skills/` |
| Gemini CLI | `.gemini/skills/` |

---

## Usage

Once installed, skills activate when you describe what you need. No commands, no configuration.

```
Find a name for my new developer tool
I need to name a B2B SaaS for supply chain teams
Audit our brand name "Acme" - we sell to enterprise HR
Map how companies in the CRM space are named
Create a naming guide for our product line
```

---

## Example output - domainforge

```
DomainForge - Developer Config Management

Archetype: DevTool / Infrastructure

1. krev.dev  93/100
   Hard consonant, 4 characters, terminal-native feel.
   No overlap with Vault or dotenv naming cluster.
   Domain: krev.dev - available (~$12/yr)
   Social: @krev - available on X and GitHub
   Trademark: clean

2. onyx.sh  89/100
   Single hard word, strong memorability, shell-adjacent TLD.
   Domain: onyx.sh - available (~$18/yr)
   Social: @onyxdev - available
   Trademark: check in software category
```

---

## Part of VeyraSkills

This pack is part of [VeyraSkills](https://github.com/veyralabsgroup/veyraskills), a collection of Claude Code skills for founders, developers, and builders.

---

## License

MIT. Built by [VeyraLabs](https://veyralabs.com).
