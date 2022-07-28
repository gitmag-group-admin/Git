
**In this session we are going to learn :**
 - Git add
 - Git commit
 - Skipping the Staging area
 - Remove files
 - Rename files

## Git add
The git add command is used to add file contents to the Staging Area. This command updates the current content of the working tree to the staging area. It also prepares the staged content for the next commit. Every time we add or update any file in our project, it is required to forward updates to the staging area.
```
$ git add file1.txt file2.txt
```
OR
```
$ git add *.txt
```
OR
```
$ git add .
```

<p align="center">
<img src="https://raw.githubusercontent.com/gitmag-group-admin/Git/main/img/88.JPG" width="750" />
</p>

## Git commit
It is used to record the changes in the repository. It is the next command after the [git add](https://www.javatpoint.com/git-add). Every commit contains the index data and the commit message. Every commit forms a parent-child relationship. When we add a file in Git, it will take place in the staging area. A commit command is used to fetch updates from the staging area to the repository.
`git config --global core.editor "code --wait"`

for short message:
```
$ git commit -m "message"
```

for complete message:
```
$ git commit
```
after this command the `vs code` will open and there we can write our messages.
in `vs code` we must type our message in two section: 
1. short description
2. long description


## Skipping the Staging area
to do this :
```
$ git commit -a -m "message"
```
OR
```
$ git commit -am "message"
```
## Remove files
```
rm file.txt
```
after this we should take the `file.txt` into staging area and after that commit it. 
we can see which files are in staging area by this command :
```
$ git ls-files
```
But we can use below command to do this without take the file into staging area :
```
$ git rm file.txt
```

## Rename files

use move command to rename files in Unix:
```
mv file.txt index.html
```
now we are going to add two files into staging area like this :
```
$ git add file.txt index.html
```
then commit it.
But git give us a better way to do this :
```
$ git mv file.txt index.html
```
by this way we are not going to use `add` command to take file into staging area. and we can commit it easier.








