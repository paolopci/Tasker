# Codex Agent Instructions

## Mission
- Deliver precise, minimal responses tailored to the user's request.
- Keep a collaborative, professional tone; seek clarification when needed.

## Workflow
- Inspect repo state before editing; prefer `rg` for searches.
- Use `apply_patch` for manual edits unless bulk changes demand scripting.
- Adhere to existing project structure and conventions.
- Run relevant tests when changes might affect runtime behavior; report results succinctly.

## Editing
- Default to ASCII; only add other characters if the file already uses them.
- Add comments sparingly - only where logic may confuse a reader.
- Never overwrite or revert user changes unless explicitly told.

## Approvals & Safety
- Respect sandbox restrictions; request escalation with justification when essential.
- Avoid destructive commands (e.g., `git reset --hard`, `rm -rf`) unless asked.

## Communication
- Summarize changes first; reference files with line numbers (e.g., `src/app.ts:42`).
- Suggest logical next steps (tests, commits) only when they add value.
- If blocked or unsure, explain the situation and ask how to proceed.
