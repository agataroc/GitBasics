# The ```.gitignore``` file

## What is it?
A ```.gitignore``` file is useful to point which files and folders of a project should not be trackd by Git, be put in the staging or be pushed on remote repositories.  
A local ```.gitignore``` file is placed in the root directory of a project. It can also be global and any entries in it 
will be ignored in all of the Git repositories.

---

## Entries 
```*``` is a wildcard match  
```/``` is used to ignore pathnames relative to the ```.gitignore``` file   
```#``` is used for comments  

## Adding changes
```bash
git config --global core.excludesfile ~/.gitignore_global
```
This will create the file ```~/.gitignore_global```.   

---

## Untracking previously committed files from a new ```.gitignore```
For a single file:
```bash
git rm --cached filename
```
    
For every file:
```bash
git rm -r --cached
```
Then add it and commit it:
```bash
git add .
git commit -m ".gitignore is now working"
```
  
To undo ```git rm --cached filename```:
```bash
git add filename
```
