# Using Blame

```bash
git blame file
git blame [commit-ID] file
```

- ```blame``` prints the latest commit ID, author info, timestamp, and the commit
message for each line in the given file

- It *cannot* tell you whether a line was added or how it changed

- It can only tell you the details about the ```HEAD``` (or the given commit)

- Furthermore, it *cannot tell you about deleted lines*

- You can also supply a branch name to blame to see the details of a file at the
```HEAD``` of that branch

- ```-s``` removes the date, time and author name from the output
