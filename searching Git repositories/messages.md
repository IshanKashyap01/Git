# Searching Commit Messages

```bash
$ git log --oneline --grep menu
d36c983 add first draft of dinner menu
99fd56e add first draft of appetizer and drink menus
```

- ```--grep``` prints only the commits whose message contains the given pattern

- It can be combined with other flags like ```--graph``` and ```--oneline``` as
well
