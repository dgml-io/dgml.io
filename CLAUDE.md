# Fork-based contribution workflow (REQUIRED)

## Git & PR policy — do NOT push branches to the upstream repo

This org uses a **fork-based** workflow for all day-to-day code changes. Never create
a branch on or push to the upstream `dgml-io/*` repository, even if you have write access.
(Claude Code's built-in default is to branch on the current repo — that default does NOT
apply here; this instruction overrides it.)

When you need to open a PR:

1. Ensure a fork under the current user's account exists: `gh repo fork --remote=false` (idempotent).
2. Add/verify a `fork` remote pointing at that fork; leave `origin` pointing at upstream for pulls.
3. Push the topic branch to **`fork`**, never to `origin`.
4. Open the PR from the fork: `gh pr create --repo dgml-io/<repo> --head <user>:<branch>`.

Do **not** run `git push origin <branch>` or a bare `git push` when `origin` resolves to
`github.com/dgml-io/*`. If you're unsure whether a remote is the upstream or a fork,
check `git remote -v` first.
