# Typical Workflow with Multiple Collaborators

## Workflow

1. Before you start to work, update your master (either ```pull``` or ```fetch```
and ```merge```)

2. Create a feature branch from the master and finish your work

3. Update your local master again and merge it into your feature branch

    - Alternatively, you can ```fetch``` and merge the RTB of the master instead

4. Now, issue a ```pull request``` in the remote to merge your work into the master

5. After it's accepted, clean up the repo by deleting your feature branch in both
the remote and local clone

## Guidelines

- Ideally, everyone should work on their separate feature branches and merge
their work into an integration branch

  - However, some tasks require more than one person to work on

  - This may lead to more than one person using the same feature branch

- Additionally, you should never add any commits to the integration branch locally

- Always clean up your repo after updating it i.e. always call ```fetch``` with
the ```-p``` flag

## When Sharing the Feature Branch

1. ```pull``` before you start your work

2. Once you're finished committing on your local, ```fetch``` from the remote

3. If the remote has diverged, ```merge``` its RTB into your local branch

4. Now attempt to push your local changes to the remote
