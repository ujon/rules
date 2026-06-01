# Project README Writer

Use this skill when creating or updating project-level `README.md` and `README.*.md` files at the repository root.

Do not use this skill for README files inside individual skill directories, such as `skills/*/README.md`.

## Rules

- Keep the README short and project-specific.
- Describe only what exists in the repository.
- Do not invent features, badges, commands, or roadmap items.
- Verify file and directory names before documenting them.
- Prefer clear sections over long explanations.
- Update only project-level README files unless the user explicitly asks for another README.
- Keep language switch links between `README.md` and `README.*.md` files.
- Treat `README.md` as the source of truth for updating `README.*.md` files.
- When a new README language is added, update the language links in every README file.

## skills.sh.json

- Use `skills.sh.json` as the source of truth for README skill listings.
- Follow the grouping titles, descriptions, skill order, and `notGrouped` placement from `skills.sh.json`.
- Document only skills that are listed in `skills.sh.json` and exist in the repository.
- Verify each documented skill against its local `SKILL.md`.
- List skills as a Markdown table under each group.
- Keep skill descriptions brief and focused on the core purpose.
- Use this table shape:

```markdown
| Skill | Description |
| --- | --- |
| [skill-name](skills/skill-name/README.md) | Short core description. |
```

## Output

Write practical Markdown that helps a new reader understand the project quickly.
