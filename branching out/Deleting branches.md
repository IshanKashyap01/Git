# Cleaning Up Branches

## Merged Branches

- Once you have merged your branches, you no longer need the merged branch

- Therefore, you should clean up your repository and delete that branch

- Recall that a branch is just a reference to a commit, hence you are just deleting
a reference

- Even if the branch is deleted, the feature branch commits can still be reachable
via the main branch

- Therefore, deleting the branch will have no consequences on your commit history

- However, you **cannot delete the branch you are on** so you must switch beforehand

```bash
$ git branch -d add-fall-menu
Deleted branch add-fall-menu (was d20cbef).
```

- The ```-d``` flag tells git that you wish to delete the given branch

- Git will print the last commit ID of the deleted branch

## Unmerged Branches

- Git will *error out* if you try to *delete an unmerged branch*

- This is because, if you were to delete this branch, its commits would no longer
be reachable

- In such a case, you have the following two options:

    1. Merge the branch before deleting

    2. Use the ```-D``` flag instead

- If you force delete this branch, git will still print its last commit ID so you
can recover it later
