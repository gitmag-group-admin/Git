# initialize Git - Git workflow - Git status

## Git init
The git init command is the first command that you will run on Git. The git init command is used to create a new blank repository. It is used to make an existing project as a Git project.
The git init command creates a .git subdirectory in the current working directory.

### Creating the first repository

Git version control system allows you to share projects among developers. For learning Git, it is essential to understand that how can we create a project on Git. A repository is a directory that contains all the project-related data. There can also be more than one project on a single repository.  
We can create a repository for blank and existing projects. Let’s understand how to create a repository.

```
$ git init
```

## Git workflow

<p align="center">
<img src="https://raw.githubusercontent.com/gitmag-group-admin/Git/main/img/8.JPG" width="750" />
</p>

## Git status

The git status command is used to display the state of the repository and staging area. It allows us to see the tracked, untracked files and changes. This command will not show any commit records or information.  
Mostly, it is used to display the state between **Git Add** and **Git commit** command. We can check whether the changes and files are tracked or not. Let’s understand the different states of status command.
```
$ git status
```

we are going to check status when:

1.  Working Tree is cleaned
2.  a new file is created
3.  an existing file is modified
4.  a file is deleted



