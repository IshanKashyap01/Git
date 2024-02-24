# Tags (remember me forever)

```bash
git tag name [commit-ID]
```

- `tag` is similar to branch as it is a reference to the commit ID provided
to it, which is by default, the current `HEAD`

- Similar to branches, they do not allow spaces, but `/`, `-` and `.` are allowed

- However, unlike branches, **they never move** i.e. they forever refer to the same
commit

- They are used to *mark landmarks* in a project, like a version or a commit that
fixed a nasty bug

- `-l` shows all the tags in the repository

- You can `fetch` or `push` tags with the `--tags` flag

- Just like a branch, if you have a tag pointing to a commit, it'll always be *reachable*

- Even if it has no branch or child commit pointing to it
