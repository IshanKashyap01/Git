# States of a File in Git

A file can move through various stages but could be in multiple stages simultaneously.

## Untracked

When the file is first created and is yet to be added to the ```index```

## Tracked

When the file is either committed before or just added to the ```index```

### Staged

- When the file is added to the index

- If this is the first time its added, it is now also *tracked* by git

### Unmodified

When the staged file is committed

### Modified

When the tracked file is changed but not yet added to the index
