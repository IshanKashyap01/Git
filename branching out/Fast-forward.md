# Fast-Forwarding

- Suppose a feature branch is created from the main branch

- After a few commits, the feature is complete and needs to be merged into the
main branch

- Now suppose the main branch has not changed since the inception of this feature
branch

- In such a case, the main branch will just move to the last commit of the feature
branch

- Such a merger is called a **fast-forward** merge

- It is the *best-case scenario* for mergers as there is no potential for conflicts

## Example

```bash
$ git merge add-fall-menu 
Updating a266b56..d20cbef
Fast-forward
 fall-menu.md | 16 ++++++++++++++++
 1 file changed, 16 insertions(+)
 create mode 100644 fall-menu.md
```

- Here, the ```add-fall-menu``` branch was one commit ahead of the ```master```
branch

- However, suppose we were to merge the ```master``` branch into the ```add-fall-menu```
branch:

```bash
$ git merge master
Already up to date.
```

- **Nothing happened** as the ```add-fall-menu``` branch was already ahead of the
```master``` branch
