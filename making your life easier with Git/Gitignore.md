# Tell Git to Ignore Certain Files & Folders

- There are often some files and folders that you do not wish to track

- You can tell Git to just ignore them by putting their names inside a `.gitignore`
file

- Once you've added a file to the `.gitignore`, it will no longer be shown in
`status` and cannot be `staged`

## Global Gitignore

- You can create a global `.gitignore` file to ignore files in all repositories

```bash
git config --global core.excludesfile /path/to/global/.gitignore
```

- However, you'll have to add the global `.gitignore` file to your global configurations

## Local Gitignore

- To create a local `.gitignore`, create the file in the root directory of your
repository

- After creating it, you should add it to the index and commit it

- This way it will become consistent among all contributors and you can track any
changes made to it

- If you want to ignore an already committed file:

    1. You'll delete it using the `git rm` command and commit the changes

    2. Then add it to the `.gitignore` file and commit again
