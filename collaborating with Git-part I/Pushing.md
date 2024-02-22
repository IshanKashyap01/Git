# Uploading Your Changes to The Remote Repository

## Configure Your Push Settings

```bash
$ git config --global push.default simple
$ git config push.default
simple
```

- Before you start pushing, make the above configuration change

- The ```simple``` option of ```push``` means only the commits of the current branch
will be pushed to the remote

- Although the `push```` configuration is usually simple by default it's better
to be safe than sorry

- There are four other options with the push that you can check out, however, simple
will cover most use cases

- Therefore, it is recommended that you keep this setting

## Pushing Your Changes

```bash
git push # or git push origin/remote
```

- The ```git push``` command allows you to synchronize your local changes with
the remote

- Every time you push, you'll be asked for your password by GitHub and you must
provide it with a ```personal access token```

- You can add your credentials to git via the ```credential.helper``` configuration
or by using any other credential manager

- This way, you can push w/o giving your ```personal access token```

### Public vs Private Commits

- Your *local* commits are private as you can change them (amend or reset) however
you like

- However, once you *push* them to the remote repository they become public

- It means that if you *change a public commit*, git will *reject your push*, telling
you the two commit histories don't line up

## Pushing a Local Branch

```bash
git push --set-upstream origin local-branch
# or
git push -u origin local-branch
```

- The remote will have both parents of the merge commit but it won't have the
feature branch

- However, you can update the remote to track your local branch as well

- You have to also specify the remote for which you have to set an upstream branch

- This is because you can have multiple remotes for your repositories
