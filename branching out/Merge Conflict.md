# Merge Conflict

- A ```merge conflict``` occurs during a ```merge commit``` when one or more files
are changed at the same line(s)

- That is, if the same line(s) in the same file is different in the parent commits,
a ```merge conflict``` will arise

- In such a case, git will error out and ask you to resolve the conflict before
trying again

- Moreover, it will edit your file to show and highlight the conflicts

- Now, you have the following four choices:

    1. Accept the incoming change (feature branch)

    2. Accept the current change (master branch)

    3. Accept both changes

    4. Ignore both changes and write a completely new one altogether

## Example

```bash
$ git merge improvisation 
Auto-merging tribute.md
CONFLICT (content): Merge conflict in tribute.md
Automatic merge failed; fix conflicts and then commit the result.
```

- This is what will happen if you merge two branches but a conflict occurs

```bash
<<<<<<< HEAD
There's a version-control tool called Git
For software it's an excellent fit
If your attitude ranges
Feel free to make changes
======
There's a version control tool called Git
When you feel like you just want to quit
Go and try something new
You can track what you do
>>>>>>> improvisation
```

- Your file will be edited by git to highlight the conflicts and the changes

```bash
$ git status
On branch master
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   tribute.md

no changes added to commit (use "git add" and/or "git commit -a")
```

- Moreover, the result of the ```git status``` command will now look like this

```bash
$ git status
On branch master
All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

```

- Once you have resolved the conflicts, the ```status``` command will show what's
above

- Now, as you're still merging, all you have to do is commit the merge

```bash
Merge branch 'improvisation'

# Conflicts:
#   tribute.md
#
# It looks like you may be committing a merge.
# If this is not correct, please run
#   git update-ref -d MERGE_HEAD
# and try again.


# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
#
# On branch master
# All conflicts fixed but you are still merging.
#
```

- Once you commit, the above file will open in your default text editor if you
haven't provided any commit message
