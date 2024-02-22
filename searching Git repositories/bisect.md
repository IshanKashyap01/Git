# Using Git Bisect

- The ```git bisect``` command uses the ```binary search``` algorithm to find the
first commit that introduced a particular change (like a bug)

- It is useful when you *don't know the change you're looking for but know a*
*way to verify if it's there*

- It automates the process of finding a commit for you to inspect if the change/bug
exists or not

- All you have to do is just inspect the commits it gives you and it'll find the
commit you're looking for

## How to Use

```bash
$ git bisect start
$
$ git bisect bad
$
$ git bisect good 6b11ec8
Bisecting: 3 revisions left to test after this (roughly 2 steps)
[b6c8c826ed98583a175ea4616ba9aad48ec0b1ad] replace meat dishes with vegetarian items
$
$ git bisect bad
Bisecting: 0 revisions left to test after this (roughly 1 step)
[d36c9830823a17c42025713dcbc3bc29bbb4ce36] add first draft of dinner menu
$
$ git bisect good
b6c8c826ed98583a175ea4616ba9aad48ec0b1ad is the first bad commit
commit b6c8c826ed98583a175ea4616ba9aad48ec0b1ad
Author: Armstrong <armstrong@eventplannerz.com>
Date:   Tue Jul 13 04:25:01 2021 -0400

    replace meat dishes with vegetarian items

 appetizers.md | 4 ++--
 dinner.md     | 4 ++--
 2 files changed, 4 insertions(+), 4 deletions(-)
$
$ git bisect reset
Previous HEAD position was d36c983 add first draft of dinner menu
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
```

- Start bisecting by invoking the ```git bisect start``` command

- Tell git that the current commit is bad, then tell it any good commit

- Git will start checking out commits and you'll have to tell it whether it is
good or bad

- This will continue until Git zeroes in on the first bad commit

```bash
$ git bisect start
$ git bisect good
$ git bisect bad 6b11ec8
Some good revs are not ancestors of the bad rev.
git bisect cannot work properly in this case.
Maybe you mistook good and bad revs?
```

- However, if you tell Git that the ```HEAD``` is good and an ancestor is bad,
it won't work
