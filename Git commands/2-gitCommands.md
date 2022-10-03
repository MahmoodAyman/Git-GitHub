## start with Git

### Table of content:
- [Intialize | init ](#initialize-a-repository)
- [Staging | ADD](#staging-area)
- [Commit](#commit)
- [Git | Get Info](#git-info)
- [Discard](#discard-changes)
- [Clear Cash](#clear-cache)
- [Compare Files (diff)](#differece-between-files)
### Initialize a repository

1. first things first open a project folder in your Editor.
2. open a terminal and run the following command: 
```bash
git init 
```
this command will create a new folder called .git and will setup your project to be a git repository.

after run this command you will notice that all files in the folder have a letter *U*. that means they are not <span style="color:green">tracked</span> by git yet. 
---

### Staging area

```bash
git add "file name"
```
this command will add a file to the <span style="color:brown;">**staging area.**</span>
```bash
git add .
```
```bash
git add -A
```
```bash
git add --all
```
these commands will add all files of the project to the <span style="color:brown;">**staging area.**</span>
all of them are the same.


after run this command you will notice that all new files in the folder have a letter *A*. **that means they are <span style="color:brown">tracked</span> by git now**. 

the files already exist but have some changes will have a letter *M*. **that means they are <span style="color:brown">Modified but Indexed now</span> by git now**. 

<span style="color:red;">**warning:**</span> empty folders will not be added to the staging area and git will not track them.

---
### Commit


```bash
git commit -m "your message"
```

**staging area**: means files now are ready to be commited.

this command will commit your changes with message you wrote.

<span style="color:brown;">**commited files**</span> means that these files you can back to it and revert.

it will be like a **checkpoint!**
---
### Git Info 

```bash
git log
```

this command will show you all commits you made to make sure that you are commited the files at the right branch.

when your logs gets long you can use this command to make it shorter:

```bash
git log --oneline
```
this command will show you all commits you made in one line in a short way.

```bash
git status
```
you can look at the status of your files and see if they are tracked, modified or untracked.

--- 
### Discard changes

```bash
git restore "file name"
```
this command will discard all changes you made to the file.

```bash
git restore .
```
this command will discard all changes you made to all files. this is pretty short and easy to use.

```bash
git checkout .
```
this is an older version of git restore command. it will do the same thing.

---
### Clear Cache

```bash
git rm -r --cached .
```

after make a lot of commits may be cash run dirty and you need to clear it.
this command will clear the cache of git and will remove all files from the staging area.

--- 

### Differece between Files

```bash
git diff
```

this command will show you the difference between the file before and after Modification.


this also show you the files you deleted or change name of it.
but since renaming means deleting the old file and adding the new one, git will show you the old file as deleted and the new one as added. [see Here](/Git%20commands/Delete%20and%20Rename.md)

this command will show you all the content of the file in the Terminal and it will be hard to read.


VS Code has a great extension called [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) that will show you the difference between the files in the editor.

or without extension you can use the source control tab in VS Code to see the difference between the files.