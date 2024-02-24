# Reflog (Reference Log)

```bash
git reflog
```

- Git maintains a log called the `reflog` which is updated every time the `HEAD`
moves

- It is your *safety net* as it can help you recover an unreachable commit

- Like `stash`, `reflog` also uses a stack and is local to your repository (i.e.
it isn't shared)
