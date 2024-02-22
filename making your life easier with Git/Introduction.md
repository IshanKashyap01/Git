# Configuring Git

## Introduction

- Git has two levels of configuration viz. `global` and `local`

- Global configurations are applied to all repositories throughout the system

- Whereas local configurations apply only to the repository they were invoked
from

- Therefore, when conflicted, local configurations supersede global configurations

- Moreover, local is the *default* behavior of the `git config` command

## Installing a Configuration in Git

```bash
git config [--global | --local] option [value]
```

- You can set a configuration by giving its value after the configuration

- You can use the `--unset` flag to remove a configuration

- You can get the value of a configuration by just inputting its type (local/global)
and name

- However, you have to be in a Git repository to install a local configuration

- `-l` or `--list` lists all your configurations of the specified type

- By default, it lists all your global configurations followed by the local ones
(if any)

- `--show-origin` displays the location of the configuration file of origin for
each configuration
