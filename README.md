# Learn-Git-GitHub

This repository is a fast way to learn or review Git and GitHub.

if you want fast access to git and github commands, you can see the folders in this repository.

table of content:

- [Introduction and what is Git](#introduction)
- [install Git](#Installation)
- [start with Git](#start-with-git)


## Introduction

---

**Git** is a version control system for tracking changes in files and coordinating work in a distributed way.

it watches files and what you do and compare it with last commit.

- there are some definitions you will need to know at first:

  - **repository**: a place where you can store your code;

  - **commits**: checkpoints with messages to track changes that happen in the code;

  - **branches**: it's like a multiverse a way to organize your code;

  - **synchronization**: the process of sharing and merging code;

  - **staging area**: a temporary area where you can store your changes on code;

---

## Installation

all what you need to install Git is:

1. download the latest version of Git from these links:
   - [**Git for Windows**](https://gitforwindows.org/)
   - [**Git for Mac**](https://git-scm.com/downloads)
   - [**Git for Linux**](https://git-scm.com/downloads)
2. it's a normal installation process so you can use it right away

---

## start with Git

1. first things first open a project folder in your Editor.
2. open a terminal and run the following command: 

         git init 

>this command will create a new folder called .git and will setup your project to be a git repository.

after run this command you will notice that all files in the folder have a letter *U*. **that means they are not tracked by git yet**. 


        git add "file name"
>this command will add a file to the staging area.

        git add .
        git add -A
        git add --all
>this command will add all files of the project to the staging area.


*staging area means files now are ready to be commited.*

        git commit -m "message"
>this command will commit your changes with message you wrote.

*commited files means that these files you can back to it and revert.*