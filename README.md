# How to Sync a Fork with Conflict

Simple steps to sync your forked repository when conflicts occur.

## Steps

1. Add upstream remote
```bash
git fetch upstream
```

2. Start rebase
```bash
git rebase upstream/main
```

3. Resolve conflicts
- Edit conflicted files
- Then:
```bash
git add .
git rebase --continue
```

4. Force push to update your fork
```bash
git push --force
```

## Notes
- Make sure to backup your changes before force push
- Only use `--force` on your personal branches

[Reference](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork)
