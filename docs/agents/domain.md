# Domain Docs

How engineering skills consume this repo's domain documentation when exploring the codebase.

## Before exploring, read these

- **`GLOSSARY.md`** at the repo root.
- **`docs/adr/`**: read ADRs that touch the area you're about to work in.

If either doesn't exist, proceed silently. The `/domain-modeling` skill creates domain docs lazily when terms or decisions are resolved.

## File structure

This is a single-context repo:

```text
/
├── GLOSSARY.md
└── docs/adr/
```

## Use the glossary's vocabulary

When output names a domain concept—in an issue title, refactor proposal, hypothesis, or test name—use the term defined in `GLOSSARY.md`. Don't drift to synonyms the glossary explicitly avoids.

If a needed concept isn't in the glossary, reconsider whether it belongs to the project's language or note the gap for `/domain-modeling`.

## Flag ADR conflicts

If output contradicts an existing ADR, surface that explicitly rather than silently overriding it.
