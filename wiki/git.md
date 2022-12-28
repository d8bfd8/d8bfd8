## Atomic Commit

- An atomic commit’s message is easily ≤ 50 chars
- An atomic commit makes git revert concise
- An atomic commit makes git bisect useful

## Fix Up Commits

`git commit --fixup <commit> && git -c sequence.editor rebase --interactive --autosquash <commit>~`

## Rebase Merges

`git rebase --rebase-merges=rebase-cousins origin/main`
