# Skills for Frills

A small collection of conversational skills for AI agents. The skills follow
the open Agent Skills format and can be installed with the `skills` CLI.

## Included skills

### `rubber-duck`

Guides a user through their own reasoning with focused questions, reflections,
and what-if prompts without immediately providing a finished solution or code.

### `good-bad-cop`

Examines a question through two respectful roles: a constructive Good Cop and a
skeptical Bad Cop who pressure-tests assumptions and risks.

## Install

List the skills available from a published repository:

```sh
npx skills add rgilsimoes/SkillsForFrills --list
```

Install both skills for Codex:

```sh
npx skills add rgilsimoes/SkillsForFrills --agent codex
```

Install one skill globally:

```sh
npx skills add rgilsimoes/SkillsForFrills \
  --skill rubber-duck \
  --agent codex \
  --global
```

## Test locally

From the repository root:

```sh
npx skills add . --list
```

The command should discover `rubber-duck` and `good-bad-cop`.

## Repository layout

```text
skills/
├── good-bad-cop/
│   └── SKILL.md
└── rubber-duck/
    └── SKILL.md
```
