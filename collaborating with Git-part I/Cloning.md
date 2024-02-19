# Cloning Git Repositories

```bash
$ git clone https://github.com/IshanKashyap01/working-with-remotes.git
Cloning into 'working-with-remotes'...
remote: Enumerating objects: 6, done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 6
Receiving objects: 100% (6/6), done.
```

- The ```clone``` command sends a request to the given URL for downloading that
repo on your machine

  1. If all goes well, it creates a folder in your working directory with the
    same name as the repo (unless you specified another in the command)

  2. Then it copies the entire commit history, all branches, and a few other
    things into the ```.git``` folder it just created

  3. Finally, it uses the ```git switch``` command to switch to the same branch
    that was checked out in the original

## Properties of a Clone

- The clone and the remote are *independent* of each other

- The remote does not know it was cloned but the clone knows where it came from

- Your clone is *completely disconnected* from the remote i.e. there is no *server*
*connection*

- Therefore, you can perform any operation that you could on your local repositories
