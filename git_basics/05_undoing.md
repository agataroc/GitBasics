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
