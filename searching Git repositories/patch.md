# Using the Patch Flag of Git Log

```bash
git log -p
git log -p --word-diff
```

- ```-p``` or ```--patch``` shows the actual diff that each commit introduced

- Using the ```-p``` flag with the ```-S``` flag will print the diff of each
commit from the pickaxe

- Recall that Git's log output is in *reverse chronological order*

- Therefore, the *last* commit in the output is where the string was first introduced
in the repo
