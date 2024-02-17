# Various Operations on Your Repository

## Deleting Files

```bash
git rm file1 file2...
git rm -rf directory
```

- ```rm``` removes a file from both the repository and the index

  - Only works with tracked files

- ```-rf``` recursively deletes all the files in the directory, then the directory
itself

## Moving Files

```bash
git mv source/path/to/the/file target/path/of/the/file
git mv path/file-name path/new-file-name
```

- ```mv``` moves/renames a file in both the repository and the index

  - Only works with tracked files

## Editing Commit Messages

```bash
git commit --amend
```

- ```--amend``` replaces the tip of the branch with a new commit, with the same
contents but a different commit message

- However, if you had staged some changes to the index, they will also be committed

## Renaming Branches

```bash
git branch -m new-name
git branch -m old-name new-name
```

- ```-m``` moves/renames a branch

- If only a new name is provided, the current branch is renamed

- If you need to rename a branch without switching to it, use the second command

- The second command will also work for the current branch
