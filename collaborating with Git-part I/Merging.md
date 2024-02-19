# Merging Branches

## Local merges

This is the *recommended workflow* when you are the *only contributor* to the remote

### Workflow

1. Work on your feature branch

2. When done, merge it with the integration branch

3. Push the integration branch to the remote repository

## Pull Requests

- This is the *recommended workflow* when you are *collaborating with others*

- Instead of pushing directly to integration, you push your feature branch to
the remote

- Then you issue a ```pull request``` which will be reviewed by your fellow contributors

- If they raise an issue, you can finish working in your local repo and push it
to the remote

- The ```pull request``` will be automatically updated to incorporate your new
changes

- This way, your team can always look at your latest work and your request will
only be merged if there are no problems

- By default, GitHub will *always* create a ```merge commit``` even if a *fast-forward*
is possible

- This is because it makes it easy to identify when a merge happened in the commit
history

<!-- markdownlint-disable MD024-->
### Workflow

1. Go to ```pull requests``` and click ```new pull request```

2. Select which branch (feature) to merge into which (integration)

    - Also, select the repositories for both branches in the merger (if available)

3. Click ```Create pull request``` and add the necessary information about
the merger

4. Now, click ```Create pull request``` to finalize this request in the remote repository

    - You, or any other contributor can now review and/or merge this request

5. Now click ```Merge pull request``` to merge the branches

6. After you confirm the request, you should delete the feature branch
