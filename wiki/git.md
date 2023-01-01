## Atomic Commit

- An atomic commit’s message is easily ≤ 50 chars
- An atomic commit makes git revert concise
- An atomic commit makes git bisect useful
- An atomic commit makes conflict resolution easy

## Fix Up Commits

`git commit --fixup <commit> && git -c sequence.editor rebase --interactive --autosquash <commit>~`

## Rebase Merges

`git rebase --rebase-merges=rebase-cousins origin/main`

## Separate Automated Change

Separating automated changes into a single commit and copy the command to the
commit message, e.g. `git mv` or `npx --yes prettier`, etc, reduce a lot of
effort for the reviewer, so the reviewer only need to review the command
in the commit message.
