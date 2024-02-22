# Checking Out Other Commits

```bash
$ git checkout 99fd56e
Note: switching to '99fd56e'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 99fd56e add first draft of appetizer and drink menus
```

- ```checkout``` rewrites the working directory to reflect the state of the repo
at the given commit

- Therefore, it can also be used in place of the ```switch``` command

- However, the `switch` can only change the repo to reflect the head of branches

- Whereas, ```checkout``` can be used to switch to any commit in the history
