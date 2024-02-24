# Rebase (another way to merge)

```bash
git rebase branch
```

- `rebase` reapplies the commits of the current branch over the `HEAD` of the given
branch

- In other words, it changes the commit the current branch is based on

- Therefore, the commit IDs of all the commits in the current branch are also changed

- It is particularly useful if you want to ensure a `fast-forward` merge

- However, `merge` is a simpler choice as `rebase` is much more involved and also
changes your commit IDs

- As to whether you should use `merge` or `rebase`, depends on your workflow
