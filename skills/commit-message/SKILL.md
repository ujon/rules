---
name: commit-message
description: Format Git commit messages with a one-line summary plus title-case Summary and Changes sections. Use when creating, editing, or reviewing commit messages.
license: MIT
metadata:
  author: ujon
  locale: en
  version: "1.0.0"
---

# Commit Message

## Format

```
<one-line summary>

## Summary
<1-3 sentences on motivation and context>

## Changes
- <change 1>
- <change 2>
```

## Rules

- Use `metadata.locale` for commit message content: the one-line summary, the body under `## Summary`, and the bullets under `## Changes`.
- Do not use prefix or scope tags such as `feat:`, `fix:`, or `chore:`.
- Keep `## Summary` and `## Changes` headers in English and title case.
- Explain why the change was made, not only what changed.

## Example

```
Simplify login form validation logic

## Summary
Consolidated duplicated validation branches into one place to reduce maintenance overhead.

## Changes
- Merged email/password validation into a `validateLoginInput` helper
- Removed unused `legacyCheck` function
- Unified validation failure messages under the i18n dictionary
```
