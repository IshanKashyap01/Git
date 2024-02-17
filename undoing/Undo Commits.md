# Undoing Commits

## Using Reset

```bash
git reset commit-ID
git reset HEAD~n
git reset HEAD^m
git reset HEAD^m~n
```

- ```reset``` removes all commits before the given commit

- You can reset to a commit using either its ID or reference it via ```HEAD```

### Flags with Reset

```bash
# Commit history
# A <- B
git reset --soft A # B~1
git reset A # or --mixed A
git reset --hard A
```

1. ```--soft``` moves the edits in B to the index, then from the index to the repo

2. ```--mixed``` does what soft does, then copies the edits in A to the index

3. ```--hard``` does what mixed does, then copies the edits in A to the repo

## Using Revert

```bash
# Commit history
# A <- B
git revert B
```

- ```revert``` creates and commits an anti-commit of the given commit

- Given one or more existing commits:

    1. It first calculates the reverse of their changes

    2. Then, pushes these changes as a new commit, negating the given commits

- Hence, it undoes the given commit but does not delete it from the history
