# Typical Workflow with Branches

1. Typically, base your new branches on commits from the **integration branch**

    - Integration branches reflect the work of all the branches

    - Therefore, your branch will have everything that has been completed so far

2. Merge back into the integration branch once you are done

    - Once you are done with a branch, integrate it right away

    - If you forgot something, you can always create a new branch

3. Don't reuse branches

    - A typical workflow doesn't include reusing branches instead we create a new
    branch

    - This is because branches will grow *stale* once they're done

    - However, the main branch will continue to grow as the project continues

    - Besides, creating branches is cheap as they are only references to a commit
