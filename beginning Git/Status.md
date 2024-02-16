<!-- markdownlint-disable MD026 -->
# Computer, status report!

- The ```status``` command prints the status of the working tree

- It displays all the *staged* and *unstaged* files

***Note:*** *The ```git status``` is referred to as a **safe command** as it only*
*asks for information from the repository and doesn't affect it in any way*

## Empty Repository

```bash
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
```

## After Files are Created

```bash
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Checklist.md
        README.md

nothing added to commit but untracked files present (use "git add" to track)
```

## One File is Added

```bash
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Checklist.md
```

## After a Commit

```bash
git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Checklist.md

nothing added to commit but untracked files present (use "git add" to track)
```
