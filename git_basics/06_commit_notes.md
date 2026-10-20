# Adding notes to commits

## Extended commit message
Te get a description that is separated by an empty line. You can write ```git commit``` without the m so that the Git will open the default text editor. Otherwise on terminal:
```bash
git commit -m "Commit title" -m "First line of the comment" -m "Second line etc."
```

---

## Add a npte to an existant commit
For the HEAD:
```bash
git  notes add -m "Text"
```
For a specific commit: 
```bash
git  notes add -m "Text" <commit-hash>
```

---

## Visualising notes
```bash
git notes show <commit-hash>
```

--- 

## Modifying notes before pushing to a remote repo
```bash
git commit --amend -m "New title" -m "new description"
```
or
```bash
git notes add -f -m "new note"
```

---

## Pushing notes to remote repos
```bash
git push origin refs/notes/*
```
