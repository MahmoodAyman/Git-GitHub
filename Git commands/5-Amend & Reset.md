# Change History 
### Table of Contents
- [Amend](#amend)
- [Reset](#reset)
- [Hard Reset](#hard-reset)
- [Rebase](#rebase)
---

## Amend

what if you commit a file and you want to change it without creating a new commit?
you can use `git commit --amend` command to change the last commit message or to add more files to the last commit.

```bash
git commit --amend
```
this will open the last commit message in your default text editor and let you edit the file.

after you save the file the commit will be changed.

--- 
 
## Reset
you can reset the last commit by using `git reset` command.

```bash
git reset "commit id" or "commit Hash" 
```
this will reset the changes of the commit and move the changes to the working directory.



**Remember!** to get commit id you can use [git log](/Git%20commands/2-gitCommands.md#git-info) command.


this will not delete the files but will rewind the commit.
so if you write `git log` command will see that the commit you reset is not there anymore.
--- 

## Hard Reset

this command is a little bit deangerous! 
```bash
git reset --hard "commit id" or "commit Hash" 
```
this command will delete the commits before the commit ID you reset to.
and will delete the files from the working directory. 

--- 

## Rebase

rebasing is another way to travel back in time.
and it's designed to take a commits from one branch and apply them to another branch.

```bash
git rebase "branch name" or "commit id" or "commit Hash" 
```
```bash
git rebase -interactive "branch name" or "commit id" or "commit Hash" 
```
this will open the commits in your default text editor and let you edit the file.
**this is the best way to use rebase command.**

```bash
git rebase -i HEAD~3
```
this will move back to a certain number of commits. 
in our case it will move back to 3 commits.

```bash
git rebase -i --root
```
this will bring you back to the first commit.

here you can take the last commit and paste it to the top of the file and save the file and the commit will be moved to the top!    