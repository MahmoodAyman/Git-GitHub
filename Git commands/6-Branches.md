# Branches 
one of the powerful features of git is the ability to create branches.

```bash
git branch
```

this command will show you all branches you have in your project.

### Table of Contents
- [Create and Switch](#create-or-switch-branches)
- [Merge](#merge-branches)
- [Delete](#delete-branches)
- [Git Flow](#git-flow)
---
## Create or Switch Branches

```bash
git switch -c "branch name"
```
this command will create a new branch and switch to it.

this new branch will be a copy of the branch you are in with the same files and commits.

```bash
git checkout -b "branch name"
```
this is an older version of the previous command `switch command`.

```bash
git switch "branch name"
```
this command without `-c` will switch to the branch you want and alreay exists.

--- 

## Merge Branches
this is a way to merge two branches together.

for example if you work in a branch and you want to merge it with the main branch.

```bash
git merge "branch name"
```
this command will merge the branch you are in with the branch you specified by the name.
--- 

## Delete Branches
if you create a branch to work on a specific feature and you don't need it anymore you can delete it.

```bash
git branch -delete "branch name"
```
or 
```bash
git branch -d "branch name"
```
this command will delete the branch as long as the branch is free of conflicts.

may be you see the previous command with a `-D` instead of `-d` this forces git to ignore conflicts and delete the branch.

```bash
git branch -D "branch name"
```
---

## Git Flow
this is a way to organize your branches and make it easier to work with them.
1. First you create a branch to work on a feature or fix a bug.
2. make changes to that branch and commit them.
3. switch to the main branch and merge the branch you were working on.
4. delete the branch you were working on.

this is a general pattern but it may be has some changes depending on the project.
