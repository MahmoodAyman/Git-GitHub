# Git 

### what is Git?

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
   - [**Download Git**](https://git-scm.com/downloads)
2. it's a normal installation process so you can use it right away

---

all you need after that is just an Editor and a terminal.

---

your default branch is **main**.
older versions of git use **master** as default branch.

every commit you make will be on the main branch and has a unique id.

--- 
### Git Environment
Git has three Places where you can move your files:
1. **working Environment**: here where is the file you are working on and has the last commit you did.
2. **staging area**: here where you can store your changes before commiting them
    this is an temporary area like dating someone before you marry them^^.
3. **commit**: here where you can store your changes permanently.
here is a new log entry for your changes.

--- 

### File Status
before commit files it may have one of these status:
1. **untracked**: means that git doesn't know about this file yet.
any new files you added since the last commit will be untracked.
2. **tracked**: means that git knows about this file.
    Now **Tracked** files may have one of these status:
    1. **unmodified**: means that the file is tracked but has no changes since the last commit.
    2. **modified**: means that the file is tracked and has changes since the last commit.
    3. **staged**: means that the file is tracked and has changes since the last commit and it's ready to be commited.


--- 
something important to know: 
git is always looking at your files and compare them with the last commit you made.