# Git config

Git supports a command called **git config** that lets you get and set configuration variables that control all facets of how Git looks and operates.

Items we must specify first time of installing git : 
- **Name**
- **Email**
- **Default Editor**
- **Line Ending**

## Git configuration levels
The git config command can accept arguments to specify the configuration level. The following configuration levels are available in the Git config.

<p align="center">
<img src="https://raw.githubusercontent.com/gitmag-group-admin/Git/main/img/6.JPG" width="200" />
</p>

### **System** :
The system-level configuration is applied across an entire system. The entire system means all users on an operating system and all repositories. The system-level configuration file stores in a **gitconfig** file off the system directory. **$(prefix)/etc/gitconfig** on UNIX systems and **C:\ProgramData\Git\config** on Windows. 

### **Global** :
The global level configuration is user-specific configuration. User-specific means, it is applied to an individual operating system user. Global configuration values are stored in a user's home directory. **~/.gitconfig** on UNIX systems and **C:\Users\\.gitconfig** on windows as a file format.

### **Local** :
It is the default level in Git. Git config will write to a local level if no configuration option is given. Local configuration values are stored in **.git/config** directory as a file.


## Set the Values of configurations :

**Setting username**
The username is used by the Git for each commit.
```
$ git config --global user.name "Ali Bayani"
```

**Setting email**
The Git uses this email id for each commit.
```
$ git config --global user.email "Alibayani@gmail.com"
```

**Setting editor**
You can set the default text editor when Git needs you to type in a message. If you have not selected any of the editors, Git will use your default system's editor.

To select a different text editor, such as Vim :
```
$ git config --global core.editor Vim
```
**Checking Your Settings**
```
$ git config --list
```
OR in editors use this :
```
$ git config --global -e
```

## Line Ending

<p align="center">
<img src="https://raw.githubusercontent.com/gitmag-group-admin/Git/main/img/7.png" width="400" />
</p>

**`\n`  : line feed**
**`\r` : carriage return**

for fixing it we must config **`core.autocrlf`** in git config.

if you are on windows :
```
$ git config --global core.autocrlf true
```

if you are on Linux or Mac :
```
$ git config --global core.autocrlf input
```

