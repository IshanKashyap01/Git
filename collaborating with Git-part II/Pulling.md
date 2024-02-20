# Pulling from the Remote

## Pulling Commits From Remote

```bash
$ git pull
Already up to date.
```

- The ```git pull``` command finds the remote counterpart of the branch from which
you revoked it

- Then it asks the remote repo if it has any new commits, if yes, it'll update
your local repo

## Fetching Remote Tracking Branches

```bash
git fetch
```

- ```fetch``` updates the remote-tracking branches to reflect the commit history
in the remote

- It updates all branches and commits in the remote that aren't present in your
repository

- Therefore, you get all the branches and commits that your clone didn't know about

```bash
$ git switch sangita-add-profile 
Branch 'sangita-add-profile' set up to track remote branch 'sangita-add-profile' from 'origin'.
Switched to a new branch 'sangita-add-profile'
```

- You can simply switch to them (as you would any local branch) and git will create
and switch to them

## Pull vs Fetch

- ```pull``` is ```fetch``` + ```merge``` i.e. it updates the remote tracking branch
and then merges it into the local branch

- This way you get all the changes in the remote directly to your local branch

- Whereas, ```fetch``` only updates the remote tracking branch

- This is especially useful if your remote branch has diverged from your local
