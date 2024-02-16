# What Exactly does it Mean to Commit

## How to Commit?

```bash
git add file1
git add file2 file3...
git commit -m "commit message"
```

1. ```add``` command tells git to add the given file to the index

2. ```commit``` command tells git to take a snapshot of the index

    - ```-m``` provides a message to explain the commit

## What is a Commit?

- Firstly, only the files you ```add``` are committed, i.e. **only** the changes
made to the added files will be stored

- When you ```commit```, git creates a commit object and stores it in the ```.git```
folder

- This object is stamped by a *unique identifier*, which is **computed using a**
**bunch of metadata**

- The git commit history is a ```directed acyclic graph``` or ```DAG``` for short

### What is the Commit Object?

1. The commit object only stores a **pointer** to the location where your changes
are stored

    - The folder where your changes are stored is called a **tree**

2. The **author** info i.e. your name and email address

3. The **time** the commit was made in seconds elapsed since ```January 1, 1970```

4. The **commit message** you supplied when the commit was invoked

5. The **commit ID** of the commit that came just before it

    - Not applicable for the very first commit of a repository

### How is the Commit Object?

- The chance of two commits with the same ID is less than 1 in $10^48$

- The commit object **does not store** your changes directly

- Instead, they are stored somewhere else by git

- They are stored in the binary format making it hard for humans to read but super
efficient for git
