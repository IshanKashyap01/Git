# Viewing Commit History in Git

- ```git log``` command prints the commit history of the given branch (current by
default)

- It is also a *safe command*

## Prettify the Log

```bash
git log --abbrev-commit --pretty=oneline
# Or
git log --oneline
# to display a different branch
git log [options/flags] branch-name
# to display the entire commit history
git log --all # or -a

git log --graph
```

- ```--abbrev-commit``` only prints enough characters of the commit IDs to uniquely
identify each commit

- ```--pretty=oneline``` pretty-print the contents of the log in a given format
(oneline)

- ```--oneline``` prints each log item in one line (shortened ID and message)

- ```--all``` or ```-a``` prints the entire commit history

- ```--graph``` draws a text-based graphical representation of the commit history
