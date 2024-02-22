# Searching Git Repositories with Grep

```bash
git grep pattern
```

- ```git grep``` prints every line matching the given pattern in the repository

- ```-i``` or ```--ignore-case``` ignores case differences between the patterns
and the files

- ```-n``` or ```--line-number``` prints the line number for each output

- ```-l``` or ```--name-only``` lists only the name of the files that matched

- By default, it only searches the *tracked* files

- It searches in the index and the object database instead of the working directory

- Hence, it tends to be faster than Bash's ```grep``` command
