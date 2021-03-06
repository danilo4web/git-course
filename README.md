
# Git Commands

```
# create new branch
git checkout -b branch-name

# interactive staging
git add -i

# log
git log master --oneline
```

### tag

```
# Assign a tag to a commit
git tag -a v1.1 -m "Version 1.0" dd5c49420a8

# create a tag (next commit)
git tag v0.1

# list tags
git tag --list

# list tags benning with "v2"
git tag --list "v2*"

# push tag to remote
git push origin v1.1
```
## cherry pick

##### picking a commit
```
git cherry-pick sha1
```

##### select changes
```
# between commits
git format-patch 2e33d..655da

# all the commits on the current branch to master/branch 
git format-patch master
```

## rebase
```
# rebase current branch to tip of master
git rebase master

# rebase new_feature to tip of master
git rebase master new_feature

# return commit where topic branch diverges
git merge-base master new_feature
```

## reset commit
```
# reset HEAD for sha1
git reset --hard 11e503d

# reset X commits ago
git reset --hard HEAD~1

# force push
git push -f
```
