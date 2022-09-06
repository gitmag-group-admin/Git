## Unstaging files

perhaps sometimes we have a problem in our code and we want to Unstage our files from staging area, in other words we want undo changes in our code.
so for this we can do like below: 

```git
$ git restore --staged file.txt
```
now if you see, the `file.txt` is restored from staging area.

```git
$ git reset -- file.txt
```

## Discarding local changes

```git
$ git restore file.txt
```

but for untracked files we must do like below :

```git
$ git clean -fd
```

-f : force
-d : remove whole directories
