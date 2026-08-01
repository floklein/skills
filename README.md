# Agent Skills

Reusable agent skills for focused, repeatable work.

## Available skills

### Viral Tweet Writer

Draft, rewrite, critique, and generate variants of concise X posts. The skill turns one sharp claim into a credible, repostable post using a `claim -> proof -> payoff` process.

[Read the skill](skills/viral-tweet-writer/SKILL.md)

## Install

From a published Git repository:

```sh
npx skills add <repository-url> --skill viral-tweet-writer
```

From a local clone:

```sh
npx skills add . --skill viral-tweet-writer
```

List the skills available in the repository:

```sh
npx skills add . --list
```

## Repository layout

```text
skills.sh.json
skills/
  viral-tweet-writer/
    SKILL.md
    agents/openai.yaml
    references/
```

The standard `skills/<slug>/SKILL.md` layout supports discovery through the skills CLI. `skills.sh.json` controls grouping on the repository's skills.sh page, while `agents/openai.yaml` provides Codex interface metadata. Claude Code reads `SKILL.md` and its frontmatter directly, so it requires no parallel `agents/claude.yaml` file.

## License

Licensed under the [MIT License](LICENSE).
