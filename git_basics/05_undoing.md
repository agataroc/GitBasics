#Undoing changes

## Unstage a File
To remove a file from the staging area:
```bash
git restore --staged filename.txt
```

---

## Discard Local Changes
Reverts file to last committed version.
```bash
git restore filename.txt
```

---

## Reset Last Commit 
Keeping the changes:
```bash
git reset --soft HEAD~1
```

Deleting the changes (!!PERMANENT!!)
```bash
git reset --hard HEAD~1
```

---

## Delete a Branch
To delete a *local* branch, only deletes the branch if it has already been fully merged in its upstream branch:
```bash
git branch -d feature-name
```

To delete a *local* branch, where ```-D``` option is an alias for ```--delete --force```, which deletes the branch "irrespective of its merged status"
```bash
git branch -D feature-name
```

To delete a *remote* branch:
```bash
git push origin --delete feature-name 
```
or (Git v1.5.0)
```bash
git push origin :feature-name
```
