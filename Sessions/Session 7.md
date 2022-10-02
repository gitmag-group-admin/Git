# Branching and merging
A branch is a version of the repository that diverges from the main working project. It is a feature available in most modern version control systems. A Git project can have more than one branch. These branches are a pointer to a snapshot of your changes. When you want to add a new feature or fix a bug, you spawn a new branch to summarize your changes. So, it is complex to merge the unstable code with the main code base and also facilitates you to clean up your future history before merging with the main branch.

![enter image description here](https://raw.githubusercontent.com/gitmag-group-admin/Git/main/img/eev37hwxalgf019j42a9.webp)


![enter image description here](https://raw.githubusercontent.com/gitmag-group-admin/Git/main/img/branch%203.PNG)

## list branch

using `$ git branch` or `$ git branch --list` commands we can see all the branches on our project.

## create a new branch

using `$ git branch <name>` command, we can make a new branch to work on it.

## checkout vs switch

You can switch between two branches with the **git checkout** command. To switch between the branches, below command is used:

```
$ git checkout <branch name>
```
but this way is wholy.(kolli)
its better to use `switch` command like below:

```
$ git switch <name>
```

## rename branch

We can rename the branch with the help of the **git branch** command. To rename a branch, use the below command:

```
$ git branch -m <old name> <new name>
```

## delete branch

You can delete the specified branch. It is a safe operation. In this command, Git prevents you from deleting the branch if it has unmerged changes. Below is the command to do this.

```
$ git branch -d <name>
```

## merge

Git allows you to merge the other branch with the currently active branch. You can merge two branches with the help of **git merge** command. Below command is used to merge the branches:

```
$ git merge <name>
```



