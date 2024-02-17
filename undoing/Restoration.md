# Undoing Changes

```bash
git restore file1 file2...
git restore --staged file1 file2...
```

- ```restore``` discards the unstaged (but tracked) changes and restores the
contents of the specified files in the repository from the index

  - In other words, rewrites the repo with the index

  - Cannot operate on an untracked file

  - *Opposite* of the ```git add``` command

- ```--staged``` restores the specified files in the index to the ```HEAD```

  - In other words, undoes the ```add``` command

  - *Opposite* of the ```git commit``` command
