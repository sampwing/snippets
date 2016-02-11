# Revert a pushed merge

You can revert a pushed merge by finding the sha in the log.

```
> git log
commit f18c734092db6fd966eeeadce53806ac33f10bb6
Merge: 52f22fc f3c5708
Author: Sam Wing <sampwing@example.com>
Date:   Wed Feb 10 12:37:33 2016 -0800

    Merge branch 'feature-xyz' into develop

commit f2c5708d2b568770c125f992660d0f2f3a4ab5f4
Author: Sam Wing <sampwing@example.com>
Date:   Wed Feb 10 12:37:24 2016 -0800

    Super cool feature xyz
```

We determine we want to revert the merge caused by commit `f18c73409`


```
git revert -m 1 f18c73409
```
