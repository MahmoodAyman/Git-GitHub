# Delete and Rename Files managed by Git

## Delete

acctually, you can just delete files from your local machine normally :"D 


just go to the folder, right click on the file and click delete or use the shortcut on your keyboard.

**watch out!** Git treate deleted files as something you need to add into the staging area and commit it.


don't forget you can resotro file by *restore* command.
```bash
git restore "file name"
git restore .
```

the other way to **delete** files is to use command line:

```bash
git rm "file name"
```
**watch out!** this command will delete the file from your local machine and from the staging area.
so you don't need to add it to the staging area.

so this save us a step.

but to restore this file you need to add a little bit of code to the command:

```bash
git restore --staged "file name"
git restore --staged .
```
or 
```bash
git restore -S "file name"
git restore -S .
```

this will restore the file from staging to the working directory.

now the file recorded as deletion but restored from staging area.

again, use restore command but without the *--staged* or *-S* to restore the file from the working directory to the staging area.

```bash
git restore "file name"
git restore .
```
---

## Rename

just like deletion you can simply rename the file from your local machine.

but **watch out!** Git treate renamed files as completely new files and will not stage them automatically! 

first it will delete the file with the old name 
and then it will add the file with the new name!

now using *git restore* will return back the old file but still keep the new file also.
that means you have two files with the same content! 

so you need to restore old file and delete the new file manually.

```bash
git restore "old file name"
git rm "new file name"
```

another way to rename files is to use command line:

```bash
git mv "old file name" "new file name"
```
this command will rename the file from old name to new name and add it to the staging area.