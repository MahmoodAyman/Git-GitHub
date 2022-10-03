## Ignoring Files 
you may be have a sensitive file that you don't want to share... may be a password or an API key.

to take care of these files you can use `.gitignore` file.

inside this file you can write the name of the files you don't want to share.

if you want to ignore folder you can write the name of the folder and add `/` at the end of the name.

```bash 
git config --global core.excludesfile [file]
```
if you have more than one project you can use this command to configure a global `.gitignore` file.

whenever you create any project this file will be ignored automatically.
