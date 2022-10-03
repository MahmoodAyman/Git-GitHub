# GitHub
github is an online service that helps you to share your code with others and collaborate with them on the same project.

essentially, github is a storage service that allows you to store your code online and share it with others.

everything you learned about git is applicable to github.

### table of contents
- [what is github](#what-is-github-used-for)
- [Start using github](#start-using-github)
- [create a repository](#create-a-new-repository)
- [clone a repository](#tie-it-to-your-local-repository)
- [Pull requests](#pull-changes-from-your-remote-repository)

## What is GitHub used for?
1. github is used to store your code online and share it with others.
2. it offers a lot of tools for tracking your code and collaborating with others.
3. it's has a lot of project management tools.
    you can create issues and assign them to developers that works with you.
--- 

## start using GitHub 
I assume since you are reading this you already have a GitHub account^^

1. you need to create a new repository.
2. tie it to your local repository.
3. push changes to your remote repository from your local repository.
--- 
## create a new repository
1. go to your GitHub account.

    simply you can go to your account and click on the **new** button.

    or you can wirte in url bar: `https://github.new` and it will take you to the same page.  

2. write a **name** for your repository 

             name of repositery must be not repeated in your account.(you can't have two repositories with the same name)

3. write a **description** for your repository

            description is optional but it's a good practice to write one.

4. choose a **visibility** for your repository

    you can choose between two options:
    1. public

             public repositories are free and anyone can see them.
    2. private

             private repositories are paid and only you and your collaborators can see them.

5. you can initialize your repository with a different files 
    1. you can add **Readme** file

             readme file is a file that contains information about your project.

    2. you can add **gitignore** file
    
           gitignore file is a file that contains a list of files that you don't want to track.

    3. you can add **license** file
    
            license file is a file that contains the license of your project.


6. click on **create repository** button

---

## tie it to your local repository (clone a repository)

1. go to your local repository and open the terminal.
2. copy the url of your remote repository.
3. write the following command in your terminal:

```bash
git remote add origin <url of your remote repository>
```
this is to set remote conection repository to your local repository.

you can use another command to do the same thing:
```bash
git clone <url of your remote repository>
```
this command will clone your remote repository to your local machine.

---
after you add files to staging area and commit them you can push them to your remote repository by writing the following command:
4. push your changes to your remote repository.

```bash
git push -u origin main
```
this command will push your changes you have commited to your remote repository.

```bash
git push --set-upstream origin main
```
this is the longer version of the previous command. 

```bash
git push --all
```
this command will push all your branches to your remote repository.

--- 
sometimes when you want to push a branch to your remote repository GitHub will ask you to push it manually.

to do that you need to write the following command:
```bash
git push --set-upstream origin <name of your branch>
```
---
## pull changes from your remote repository
when you want to pull changes from your remote repository to your local machine 
to start working on it from where you left off you need to write the following command:

```bash
git pull origin main
```
this command will pull changes from your remote repository to your local machine.

```bash
git pull --all
```
this command will pull all your branches from your remote repository to your local machine.

---

**the same thing can be done by writing the following command:**
```bash
git fetch origin main
```
this command will fetch changes from your remote repository to your local machine.

```bash
git fetch --all
```
this command will fetch all your branches from your remote repository to your local machine.

