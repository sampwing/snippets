# Show changes in files between commits

When merging or deploying code is it often useful to compare the most recent commits with the last commit that was deployed.  Say the most recent commit was `80763b2` and we want to see what files will be modified when deployed to `origin/master`.

```
$ git diff --name-status 80763b2..origin/master
M       .gitignore
D       .gitignoreasx
A       README.md
```

Gives you something useful which indicates which files have been (a)dded, (d)eleted or (m)odified.
