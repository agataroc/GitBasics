# Branching

## View Branches
Lists local branches.
```bash
git branch
```

---

## Create a New Branch
```bash
git branch feature-name
```

---

## Switch Branch
To start working on said branch.
```bash
git checkout feature-name
```

Or (modern command):

```bash
git switch feature-name
```

---

## Create and Switch in One Command

```bash
git checkout -b feature-name
```

---

## Merge Branch into Current Branch
Combines branch changes into the current branch.
```bash
git merge feature-name
```

To see what we've merged in so far:
```bash
git branch --merged
```

---

## Push a Branch to Remote
```bash
git push -u origin feature-name
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
---
