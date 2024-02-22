# Git Log's Pickaxe Capability

```bash
git log -S string [file]
git log -G pattern [file]
```

- ```-S``` shows the commits that added/removed the given string in the entire
repository

- ```-G``` shows the commits whose patch text contains the given pattern

- You can limit the search to a single file by supplying the path to that file

- While the ```blame``` command searches one file, the pickaxe searches the
entire repo
