# HEAD in Git

- Recall that a branch always refers to its latest commit

- ```HEAD``` is the reference to the current branch

- Therefore, it is an indirect reference to the latest commit of the current
branch

## Navigating the Commit History via Head

- You can refer to previous commits relative to the head using the ```~``` operator

- Note that ```HEAD~``` is an alias for ```HEAD~1```, which is the commit right
before head

- You can refer to any commit that came before by ```HEAD~n``` where ```n``` is
the nth generational ancestor of head

- If it refers to a ```merge commit```, its parents can be accessed via the ```^```
operator
