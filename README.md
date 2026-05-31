# naming-suite — Brand & Naming Intelligence for Claude Code

Four skills that work together to name products, audit brands, map competitors, and build naming systems.

```bash
npx @veyralabs/skills install naming-suite
```

---

## Skills

| Skill | What it does |
|-------|-------------|
| [`domainforge`](./domainforge/SKILL.md) | Generate and score startup names. Domain availability, social handles, trademark check, brand narrative |
| [`brandaudit`](./brandaudit/SKILL.md) | Audit an existing brand name across 8 dimensions. Severity scoring, rebrand verdict |
| [`competitornames`](./competitornames/SKILL.md) | Map the naming landscape in your market. Saturation levels, whitespace, naming brief for DomainForge |
| [`namingguide`](./namingguide/SKILL.md) | Generate a complete naming guide for a company or product line. Principles, system, dos/don'ts, approval checklist |

---

## Recommended flow

```
competitornames → domainforge
brandaudit      → namingguide
```

Run `competitornames` first to map the competitive landscape, then `domainforge` to generate names that stand out from it.
Run `brandaudit` on an existing name, `namingguide` to lock in what works.

---

## Usage

Once installed, activate in any Claude Code session — skills trigger contextually.

**DomainForge:**
```
Find a domain for my new SaaS
Name my CLI tool for environment variables
What should I call this project?
```

**BrandAudit:**
```
Audit the brand name "Acme" for a B2B SaaS
Is our brand name working?
```

**CompetitorNames:**
```
Map the naming landscape for developer config tools
Who are my competitors and how are they named?
```

**NamingGuide:**
```
Create a naming guide for our company
We're building a product line and need naming conventions
Our feature naming is inconsistent — generate a guide
```

---

## Example Output — DomainForge

```
DomainForge Analysis — Developer Config Management

Archetype: DevTool / Infrastructure
Mode: Indie Hacker

Top Recommendations

1. krev.dev — 93/100
   Hard consonant, 4 chars, terminal-native in lowercase.
   Zero overlap with Vault/dotenv cluster. Premium DevTool energy.
   Domain: krev.dev — available (~$12/yr Porkbun)
   Social: @krev — available on X, GitHub
   Trademark: Clean

2. onyx.sh — 89/100
   Single hard word, immediate memorability, shell-adjacent TLD.
   Domain: onyx.sh — available (~$18/yr)
   Social: @onyxdev — available
   Trademark: Check in software category
```

---

## Installation

```bash
# Via veyraskills CLI
npx @veyralabs/skills install naming-suite

# Install individual skill
npx @veyralabs/skills install domainforge

# Or copy manually to your agent's skills directory
# Claude Code: .claude/skills/
# Cursor:      .cursor/skills/
# Windsurf:    .windsurf/skills/
```

---

## Part of VeyraSkills

This pack is part of the [VeyraSkills](https://github.com/veyralabsgroup/veyraskills) collection — a curated set of Claude Code skills for founders, developers, and AI builders.

---

## License

MIT — Built by [VeyraLabs](https://veyralabs.com)
