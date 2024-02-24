# Cherry Picking (copying commits)

```bash
git cherry-pick commit-ID
```

- `cherry-pick` picks the given ID and places it on top of the current branch

- The commit ID of the cherry-picked commit will be changed

- This is only useful when you have a bug fix on your feature branch that you
want to make available to everyone

- However, other changes in your branch are not ready to be merged yet

- The best way to integrate your changes is to merge your feature branch into
an integration branch

- Cherry-picking commits should be only used as a *last-ditch* effort
