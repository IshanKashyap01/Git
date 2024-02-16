# Branches in Git

- When you create a new branch, it will be based on the branch you were on at
that time

- A branch is just a *reference* to a commit via its ID

- This reference is updated every time you make another commit on that branch

## Creating a Branch

```bash
$ git branch
* master
$ git branch add-fall-menu
$ git switch add-fall-menu 
Switched to branch 'add-fall-menu'
$ git branch
* add-fall-menu
  master
```

1. ```branch``` lists out all the branches in the repositories

2. ```branch "name"``` creates a branch with the given name

3. ```switch``` rewrites your repository to reflect the last commit on the given
branch

### After Making a Commit

```bash
$ git status
On branch add-fall-menu
nothing to commit, working tree clean
```

### *Note:*

- The ```git branch``` is a *safe command* just like ```status``` except it lists
out all the branch names

- You can create and switch to a branch with the ```switch``` command as follows:

```bash
git switch -c my-first-branch
```
