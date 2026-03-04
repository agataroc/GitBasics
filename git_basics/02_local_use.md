# Creating a Repository

## Initialize a new repo
Creates a new empty Git repository in the current directory.
```bash
git init
```

---

## Clone an existing repo
Downloads a remote repository to your local machine.
```bash
git clone https://github.com/username/repository.git 
```
//github might be eplaced by gitlab

---

## Check a repo's status
Shows:
- Modified files
- Staged files
- Untracked files
```bash
git status
```
---

## Adding files to the staging area 
To add a single file to the staging area of the current directoy:
```bash
git add filename.txt
```
To add all files:
```bash
git add -A
```

---

## Removing files from the staging area
```bash
git reset filename -- path/to/file
```

---

## Commit staged changes 
Saves the staged changes to the repository history.
```bash
git commit -m "commit message"
```
//the commit message should be a detailed description of what you changed, but not longer than a sentence

---

## Removing a commit 
To undo a commit and save your work:
```bash
git reset --soft HEAD~1
```

To remove the commit completely and go back to the most recent one before:
```bash
git reset --hard HEAD-1
```

To modify the last commit:
```bash
git commit --amend
```

---

## Keeping track of the commits
To keep track of all the last commits.
```bash
git log
```

To go back and work on a certain log:
```bash
git checkpoint logname
```
