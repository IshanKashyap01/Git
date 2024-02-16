# Merge Commit

- Suppose, we have a feature branch and a master branch and the feature branch
is ready to be merged

- However, *new commits* were made to the master branch in the time being

- Now git will need to somehow merge the changes of two different lines of work

- To do this, **git** will create *a new commit* from the last commits of the
two branches

- This commit is different in the sense it will have **two parents** instead

- The first parent will be from the master and the second, from the feature

- If such a merger is possible, all you'll need to do is provide a commit message

## Example

```bash
$ git merge add-thurs-menu 
Merge made by the 'ort' strategy.
 thursdays-menu.md | 16 ++++++++++++++++
 1 file changed, 16 insertions(+)
 create mode 100644 thursdays-menu.md
```

- This is what will happen when you merge two diverged branches

```bash
Merge branch 'add-thurs-menu'
# Please enter a commit message to explain why this merge is necessary,
# especially if it merges an updated upstream into a topic branch.
#
# Lines starting with '#' will be ignored, and an empty message aborts
# the commit.
```

- If you didn't provide a commit message, a file with the above content appears
in your default editor
