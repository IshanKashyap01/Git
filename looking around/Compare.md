# Compare Changes in Your Files

```bash
git diff --word-count
```

1. ```diff``` command shows changes b/w commits, commit & working directory, etc.

    - It prints only the hunks with changes, line-by-line

    - Short for *difference*, it is also a *safe command*

2. ```--word-count``` prints the changes word-by-word instead

## Comparing Changes in Files

### Unstaged Changes

- ``diff`` compares the staged and unstaged changes in the index and working directory

- The version in the *index* is treated as *old* and the *working directory*
as *new*

### Staged Changes

```bash
git diff --cached # or --staged
```

- ```--cached``` compares the *object database with the index*

- That is, changes in the *index* are *new* whereas the *object database* is the
*old* version

## Comparing Branches

```bash
git diff old-branch new-branch
```

When you switch branches, the *index* is also rewritten along with the working
directory

## Comparing Commits

```bash
git diff commit-ID-1 commit-ID-2
```

You can compare any two commits in the history regardless of their positions in
the commit history
