# Remote Tracking Branches

- The ```git clone``` command doesn't just copy-paste the remote repository

- It also creates a set of branches with the same name as their remote counterparts

- However, they have the name of the remote prefixed to them

- After cloning, your branches point to the same commit as their remote counterparts

## Properties

1. They are git's bookmarks, so git knows what to do when you push (i.e. where
to push)

2. They help you get updates from the remote

3. They can tell you if you're ahead i.e. you need to push

4. They offer a safe way to catch up to remote

    - If your local branch has diverged from its remote counterpart, you can merge
    it with its RTB

5. You have no control over them; git keeps them for housekeeping
