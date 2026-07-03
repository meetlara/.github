# CLAUDE.md

## Opening PRs

When opening a PR (`gh pr create`), populate `.github/PULL_REQUEST_TEMPLATE.md`:

- **Summary**: concrete what + why — this is Greptile's primary intent signal; avoid vague phrasing.
- Fill **Changes**, **Review focus**, **Testing**, and the **Linear** line.
- Linear: use `Closes ENG-<n>` to auto-close on merge, or `Ref ENG-<n>` to link without closing
  (use `Ref` for one of several PRs on the same issue). Name the branch `eng-<n>-<slug>` so Linear
  also auto-links.
- Promote conditional sections (Risk & rollback, Migrations, Screenshots, Related PRs, Follow-ups)
  ONLY when relevant; delete the rest.
- Never leave placeholder text, HTML-comment guidance, or empty headings in the final body.

> **Note:** This file only takes effect for agents working inside the `.github` repo. The PR
> template itself propagates org-wide, but this rule does not — mirror this "Opening PRs" section
> into each repo's own `CLAUDE.md` so Claude Code applies it everywhere.
