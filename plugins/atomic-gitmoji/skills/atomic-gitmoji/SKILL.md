---
name: atomic-gitmoji
description: Organize mixed changes into small, logical Git commits using Unicode gitmoji. Use when asked to commit changes or prepare local work for a push.
---

# Atomic Gitmoji

The developer often works on several things before committing. Turn the
in-scope work into small, logical commits that are easy to review. Preserve
the approved final behavior and unrelated pending work.

## Choose commit boundaries

- Inspect Git status, staged and unstaged diffs, and relevant untracked files.
  Existing staging can contain several unrelated tasks; assess the changes
  by purpose before creating commits.
- Group changes around one coherent behavior or concern and order the groups
  by dependency. Include the source, strings, schema changes, and other files
  needed to make each step complete.
- Split independent work into separate commits, including separate hunks of
  the same file when appropriate. Keep tightly coupled changes together.
  Choose boundaries by meaning, without an arbitrary file count or line limit.
- Stage explicit paths or selected hunks for each group. Preserve unrelated
  staged and unstaged changes, and inspect the exact staged diff before
  recording each commit. Check it for whitespace errors.

## Write commit messages

Follow the [gitmoji specification](https://gitmoji.dev/specification) using
actual Unicode emoji. Choose the emoji that describes the change's intent.

- Keep the subject under 50 Unicode characters, including the emoji and
  spaces. Use a concise imperative description without a trailing period.
- Add a body only when it helps explain the reason for the change or a
  meaningful constraint. Separate it from the subject with a blank line and
  keep every body line under 72 characters.
- Check message lengths programmatically before committing.

Examples:

```text
🏗️ Extract shared validation logic
🚧 Scaffold the settings screen
🌐 Translate search labels
```

## Finish

Report the created commits and any work left uncommitted. Push only when
the user requests it.
