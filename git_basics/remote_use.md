# Remote Repositories

## Gaining info on remote repos
To connect your local repository to GitHub (or GitLab):
```bash
git remote add origin https://github.com/username/repository.git
```

To view remote repos, it displays the connected remote URLs:
```bash
git remote -v
```

To view all the branches:
```bash
git branch -a
```

---

## After making changes
To see the changes you made:
```bash
git diff
```
### Locally:
To see modified files, staged files and untracked files:
```bash
git status
```
To stage files:
```bash
git add -A
```
To commit changes (once you push everyone will see this description, but untill you push it only saves the changes, people won't see what you changed and won't be able to pull it):
```bash
git commit -m "message"
```

### Remotely
To push changes (upload commits) to GitHub /GitLab:
```bash
git push origin master
```

To pull changes, it fetches and merges changes from GitHub /GitLab:
!! always remember to pull before pushing, as others might have worked on the same repo in the meantime
```bash
git pull origin master
```

In both cases the "origin" is the name of the remote repo and "master" is the branch.


