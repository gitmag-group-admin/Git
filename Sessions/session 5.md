﻿## short status

we can use short status command like below :
```
$ git status −s
```

| indicator | Interpretation |
|--|--|
| ? | Untracked |
| ' ' | Unmodified|
| M | Modified |
| A | Added |
| D | Deleted |


## view staged and Unstaged changes

Git diff is a command-line utility. It's a multiuse Git command. When it is executed, it runs a diff function on Git data sources. These data sources can be files, branches, commits, and more. It is used to show changes between commits, commit, and working tree, etc.

It compares the different versions of data sources. The version control system stands for working with a modified version of files. So, the diff command is a useful tool for working with Git.

```
$ git diff --staged
```
The above command will display the changes of already staged files.

```
$ git diff
```

## view history of commits

The advantage of a version control system is that it records changes. These records allow us to retrieve the data like commits, figuring out bugs, updates. But, all of this history will be useless if we cannot navigate it. At this point, we need the git log command.

Git log is a utility tool to review and read a history of everything that happens to a repository. Multiple options can be used with a git log to make history more specific.

Generally, the git log is a record of commits. A git log contains the following data:

-   **A commit hash**, which is a 40 character checksum data generated by SHA (Secure Hash Algorithm) algorithm. It is a unique number.
-   **Commit Author metadata**: The information of authors such as author name and email.
-   **Commit Date metadata**: It's a date timestamp for the time of the commit.
-   **Commit title/message**: It is the overview of the commit given in the commit message.

```
$git log
```

#### Git Log Oneline

The oneline option is used to display the output as one commit per line. It also shows the output in brief like the first seven characters of the commit SHA and the commit message.

It will be used as follows:
```
$ git log --oneline
```

reverse mode :

```
$git log --oneline --reverse
```



