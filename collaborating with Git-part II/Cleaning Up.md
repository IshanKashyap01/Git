# Cleaning Up The Repository

- Clean up your repository by deleting obsolete branches from both the local and
remote repository

- Therefore, you have to delete their local, RTB(s) and remote counterpart(s)

- You may have branches deleted only in the local and/or remote repositories

- In both cases you need to delete their remaining counterparts as well

## Cleaning Up Branches in Remote Repository

```bash
# If you have deleted one or more branches in the local repository
git push -d remote-name [deleted-branches]
```

```-d``` deletes all the listed branches from the remote repository followed
by their RTBs in local

## Cleaning Up Branches in Local Repository

```bash
git fetch -p # or --prune
git branch -d [deleted-branches]
```

- ```-p``` removes any RTBs that no longer exist on the remote before fetching

  - Also reports the deleted RTBs, if any

- If there are any deleted RTBs reported, remove their local counterparts
