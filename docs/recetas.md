# recetas

[git - the simple guide](https://rogerdudler.github.io/git-guide/)

# time travel

```bash
git checkout SHA-ID # Go back to commit ID
git checkout HEAD~1  # Go back parent
```

# pick changes before commit

```bash
git add file1 file2
git commit -m ""selected changes
```

# move from main to a branch

```bash
git checkout -b app-refactor # create a especific brach
git switch -c app-refactor # alternative

git checkout main # back on main
git switch main # back on main

git checkout - # back to last branch
git switch - # back to last branch

```

# rebase feat branch from main

```bash
git checkout main
git pull
git checkout my-branch
git rebase main # local history has changed
```

# reset

```bash
git reset --hard SHA-ID # set head to a previous commit and removes newer

```

# reverse

```bash
git revert SHA-ID # undo previous commited changes
```

# undo

```bash
git checkout -q -- filepath # undo not commited changes 
```

# happy workflow

```bash
# happy path
git checkout main
git fetch # from remote
git merge
git switch -c 1_feat_one
git commit -a -m "add new feature"
git switch - # main
git fetch # from remote
git merge
git switch - # 1_feat_one
git merge main
git switch - # main
git merge 1_feat_one
git push # to remote
```