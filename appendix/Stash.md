# Stashes (pseudo-commits)

```bash
git stash
```

- `stash` is used when you have work that you cannot commit but need to switch
to another branch

- `push` creates a stash and pushes it on top of the stack

  - it is the default behavior of the `stash` command

- `pop` applies a stash and removes it from the list of stashes

  - You can supply the `--index` tag to pop any stash you want

- `list` will show all the stashes you have created

- `apply` applies the top-most stash but does not remove it from the list

## Properties of Stash

- Unlike commits it records the current state of both your working directory and
the index

- It stuffs the changes away in a special location leaving your working directory
clean

- That is, your repo now looks like the `HEAD` and you're ready to switch branches

- Moreover, you cannot push a stash as they are local to your repo and not designed
to be shared

- It does not work on untracked files by default
