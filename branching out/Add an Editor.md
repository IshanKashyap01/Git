# Add an Editor of Preference to Git

- Suppose you don't add a commit message in the terminal or git needs to make a
commit

- In such a case, git will open a text editor for you to write a commit message

- By default, git uses ```Vim``` as a default editor but you can change it to
any editor of your choice

- Use the following command to make ```VS Code``` your default editor:

```bash
$ git config --global core.editor "code -w"
$
$ git config --global core.editor
code -w
```

1. ```config``` command tells git that you want to interact with a git configuration

2. ```--global``` flag signifies the global git configuration file

    - In case you don't supply this flag, it signifies the current working directory
